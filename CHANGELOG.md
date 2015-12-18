Release notes
=============

This file describes all the important changes introduced to the schema after
its initial `1.0.0` release.

Please note, that all changes in the `v1` branch will be backward-compatible.


Next version (unreleased yet)
-----------------------------

* We have found a bug in version `1.0.0` of the schema - it allowed for only
  a single `<description>` element to be present. This version allows for an
  unbounded number of elements.

  We have chosen to treat this change as backward-compatible, and not increase
  the the major version of the schema yet.

* Added a new value to the attachment type enumeration: `EMREX transcript`.
  See the XSD for the description of this new value.

* The previous version of the schema required for all ELMO files to include
  additional XSDs whenever the `<extension>` element was used. This limitation
  was dropped - all `<extension>` elements will now pass the validation (they
  still need to have an appropriate `xmlns` attribute though!).

* It was unclear which ISCED *type* should be used in the `<iscedCode>`
  element. The description of the element has been made more explicit to clear
  the matter.

* Updated the `example.xml` file to better reflect the changes.

* Minor changes to the "Status of this document", "Backward-compatibility
  policy" and "Schema versioning" sections of the XSD documentation. They don't
  change the overall meaning of the previously accepted contents.


Version 1.0.0
-------------

Initial release of the schema.
