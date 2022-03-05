
The ELMO XML format
===================

The ELMO XML format is the basis for the exchange of result information. 
Elmo is based on the CEN standard EN 15981-2011 EuroLMAI. 
EuroLMAI is a data model describing assessments, primarily Diplomas, 
Diploma Supplements and Transcripts of Records for higher educations.

EMREX response XML schema
-------------------------

This schema describes the XML files returned in EMREX EMP responses.

Please note that the following terms are *equivalent* throughout the EMREX
specs:

- EMREX response file,
- EMP response file,
- ELMO file.

For more information on EMREX, please visit http://emrex.eu/.


Important
---------

* The latest official version of this schema can be found here:

  https://github.com/emrex-eu/elmo-schemas/releases

  Please note, that the `master` branch **MAY** contain some changes which has
  not yet been released (and **MAY** be reverted).

* There are many important restrictions described in the XSD annotations. **All
  implementers** (and schema designers) are **REQUIRED** to read all the
  annotations carefully.
