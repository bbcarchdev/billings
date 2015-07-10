# BBC Broadcast Billings Data

http://billings.acropolis.org.uk/

This repository has been created to allow issues around the publication of
billings data as part of the Research & Education Space to be [tracked](https://github.com/bbcarchdev/billings/issues) and to allow data dumps to be
[downloaded](https://github.com/bbcarchdev/billings/releases).

## Structure

Each file (in the `n-triples` subdirectory) contains information about a
single broadcast. Its URI has the form:

    http://billings.acropolis.org.uk/UUID#id

(where `UUID` is the 32-character hexadecimal identifier used in the filename)

This broadcast event is related to information about the *version* and
*episode* that the broadcast is of, whose URIs are in the form:

    http://billings.acropolis.org.uk/UUID#version
    
    http://billings.acropolis.org.uk/UUID#episode

These are modelled using the [Programmes Ontology](http://www.bbc.co.uk/ontologies/po). Where we know that the broadcasts, versions and episodes described in
the data have other identifiers (including those in other public BBC systems),
we've expressed that using `owl:sameAs`.

The data also contains information about the abstract document describing
the broadcast, and about the concrete N-Triples serialisation of that
document:

    http://billings.acropolis.org.uk/UUID
    
    http://billings.acropolis.org.uk/UUID.nt

## Copyright and licence

Copyright © 2015 BBC.

This data is published according to the terms of the [Open Government Licence, version 3](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

The OGL 3 is a permissive open data licence which allows you to copy, use,
modify and re-publish the data provided you adhere to some conditions,
particularly relating to attributing the source of the data.

Please ensure that you have read and understood the licensing conditions before
making use of this dataset.
