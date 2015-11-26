Release notes
=============

This file describes all the important changes introduced to the schema after
its initial `1.0` release.

Please note, that all changes in the `v1` branch will be backward-compatible.


Version master (unreleased)
---------------------------

Two elements were deprecated:

    LearningOpportunitySpecification/subjectArea
    LearningOpportunitySpecification/iscedCode

in favor of the newly introduced `<classification>` element.

A recommended `<classification type='...'>...</classification>` element has been
introduced into the schema. Its specification includes a list of predefined
`type` identifiers for each of the classification systems EMREX had recognized.

Read the specification of the new element here:
WRTODO - paste a link here


Version 1.0.0
-------------

Initial release of the schema.
