# INSPIRE XML schema repository

INSPIRE XML schemas are made available in the [official INSPIRE schema repository](https://inspire.ec.europa.eu/schemas), which offers the schemas that INSPIRE resources should make use of.

### Location & Structure of the repository

The official repository of INSPIRE XML schemas is available at https://inspire.ec.europa.eu/schemas. It includes the latest releases of all XML schemas and it also archives deprecated (older) versions of the schemas to provide reference to historic schema versions and support a smooth transition in using the newer (endorsed) ones.

The repository is organised in folders and sub-folders as indicated below:

* A **first level of folders**, each of them corresponding to a specific INSPIRE general or thematic-related XML schema and named according to the abbreviated name of the XML schema defined in the data specification. As an example, the _base_ schemas are all included in the first level folder https://inspire.ec.europa.eu/schemas/base.

* A **second level of sub-folders**, included in each first level folder, named according to the corresponding versions of the XML schemas. Each sub-folder contains the corresponding XML schema files (.xsd) associated to this specific version. As an example, the first level folder of the _base_ schemas includes the sub-folders https://inspire.ec.europa.eu/schemas/base/3.2 and https://inspire.ec.europa.eu/schemas/base/3.3.

* A **sub-folder named _deprecated_**, included in each first level folder, including all the older versions of the XML schemas (i.e. versions which were endorsed and used in the past, but have been later substituted by new endorsed schemas). The structure of sub-folders used within this sub-folder follows the same second-level structure explained above.
 
The use of deprecated XML schemas is discouraged. The newly released XML schemas should be adopted by INSPIRE data providers within the shortest possible period of time, since the whole set of endorsed schemas constitutes the basis for ensuring conformance to the requirements defined in the INSPIRE Technical Guidelines. Also, the [INSPIRE Reference Validator](https://inspire.ec.europa.eu/validator) will always make use of the latest version of schemas in the tests.

Based on feedback from MIG-T, the following indicative time periods are agreed for adopting any newly endorsed XML schemas: 

* Deprecated versions should no longer be used after 2 years after a major release (corresponding to changes in the major version number)
* Deprecated versions should no longer be used after 1 year after a bugfix release (corresponding to changes in the bugfix version number)
* There should not be specific deadlines for minor releases, i.e. the deprecated minor version can still be used as long as the corresponding major version may be used. 
