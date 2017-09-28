Release notes
=============

This file describes all the important changes introduced to the schema after
its initial `1.0.0` release.

Please note, that all changes in the `v1` branch will be backward-compatible.


Next version (unreleased)
-------------------------

This is a list of changes already introduced in the `v1.2-preview` branch.
These changes are NOT officially released yet.

* Introduce optional list of `<identifier type="...">` elements in
  `<learningOpportunityInstance>` element. Previously, identifiers were allowed
  on the LOS level only (but not the LOI level). See [this issue]
  (https://github.com/emrex-eu/elmo-schemas/issues/10).

* Prepared the EMREX ELMO format to be embedded in other contexts. Replaced
  references to "NCP" and "EMREX Client" with more generic terms (which would
  properly fit in other contexts). See [this issue]
  (https://github.com/emrex-eu/elmo-schemas/issues/13).

* The `Attachment/content` element can now occur multiple times
  (`maxOccurs="unbounded"`), and it can take an optional `xml:lang` attribute.
  See [this issue](https://github.com/emrex-eu/elmo-schemas/issues/31).

* Some more predefined identifier types were mentioned - the ones used in the
  EWP (Erasmus Without Paper) project.

* Changes in `<credit>` subelements: The `<level>` element is now DEPRECATED
  in favor of the newly introduced `<qualificationLevel type="eqf">` element.


Version 1.1.0
-------------

* We have found a bug in version `1.0.0` of the schema - it allowed for only
  a single `<description>` element to be present (per LOS). This version allows
  for an `unbounded` number of such elements.

  Since disallowing multiple descriptions was just a mishap, and we believe all
  the clients will still expect multiple descriptions present, we have chosen
  to treat this change as backward-compatible, and not increase the major
  version of the schema yet.

* Added a new value to the attachment type enumeration: `EMREX transcript`.
  See the XSD for the description of this new value.

* The previous version of the schema required for all ELMO files to include
  additional XSDs whenever the `<extension>` element was used. This limitation
  was dropped - all `<extension>` elements will now pass the validation (they
  still need to have an appropriate `xmlns` attribute though!).

* It was unclear which ISCED *type* should be used in the `<iscedCode>`
  element. The description of the element has been made more explicit to clear
  this matter.

* Updated the `example.xml` file to better reflect the changes made to the XSD.

* Minor changes to the "Status of this document", "Backward-compatibility
  policy" and "Schema versioning" sections of the XSD documentation. They don't
  change the overall meaning of the previously accepted contents.


Version 1.0.0
-------------

Initial release of the schema.
