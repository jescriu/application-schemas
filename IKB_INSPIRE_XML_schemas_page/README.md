# INSPIRE XML schemas

The INSPIRE data specifications Technical Guidelines define the data models under the scope of the Directive, formalised as UML application schemas. GML application schemas (xml schemas) are derived from them as the default encoding option for all INSPIRE spatial data themes. 

INSPIRE xml schemas are made available in the [official INSPIRE schema repository](https://inspire.ec.europa.eu/schemas). INSPIRE data resources should make use of XML schemas available on it.

## INSPIRE XML schema repository

### Location & Structure of the repository

**The official repository of INSPIRE XML schemas is available at https://inspire.ec.europa.eu/schemas - It contains the last version of XML schemas endorsed by MIG**, but also archives deprecated (older) versions of the schemas for providing reference to historic schema versions and supporting a smooth transition in using the former (endorsed) ones.

The repository is **organised in folders and sub-folders** as indicated below:

* **A first level of folders, each of them corresponding to an specific INSPIRE thematic-related application schema**, and named according the abbreviated name of the application schema defined in the data specification.

* Each first level folder contains **sub-folders (second level) named according to the corresponding version of INSPIRE XML schemas**. Each sub-folder contains the corresponding XML schema files (.xsd) associated to this specific version.

### Content of the repository 

#### Last version of XML schemas endorsed by MIG
**The last version of INSPIRE XML schemas endorsed by the Maintenance and Implementation Group (MIG) are available in the repository at https://inspire.ec.europa.eu/schemas/**. Each specific application schema is effectively placed within their corresponding first level folder (named using the application schema abbreviated name). 

Validation against the set of endorsed XML schemas using the [INSPIRE Reference Validator](https://inspire.ec.europa.eu/validator) helps data providers, solution providers and national coordinators to check whether data sets meet the requirements defined in the INSPIRE Technical Guidelines. The validator also performs this check for network services and metadata.

#### Deprecated XML schemas
**Older versions of XML schemas**, which are no longer considered valid INSPIRE XML schemas but that were endorsed at a certain point in the past, **are available under the https://inspire.ec.europa.eu/schemas/deprecated/ folder of the repository**. The structure used within this special folder for deprecated XML schemas follows the same structure of folders and sub-folders explained above.

#### Additional contents
TO BE CONSIDERED - TEXT INCLUDED BY HEIDI AT https://github.com/INSPIRE-MIF/application-schemas#readme [
The official repository also contains contains XML schemas used in the Extended Capabilities section of INSPIRE spatial data (WxS) services based on Open Geospatial Consortium (OGC) standards. ]

TBD - If considered the lastest comment: Inform where these additional schemas are accessible.

### Rules applied in versioning INSPIRE XML schemas
The version assigned to an INSPIRE XML application schema adheres to the **'X.Y.Z' pattern**, where:

* **'X' is the major version number - Updates of this number** (e.g. 3.x --> v4.0) **are applied when there are changes or new addings to the applicable legal framework (e.g. Implementing Rules) which introduce breaking (i.e. non-backwards-compatible) changes in the XML schemas**. 

Examples of these non-backwards compatible changes include e.g. adding or removing mandatory properties or changing the types or names of existing properties.

Existing data valid according to the older schema will no longer be valid according to the newer schema.

* **'Y' is the minor version number - Updates of this number** (e.g. 3.0.x --> v3.1) **are applied when non-breaking (i.e. backwards-compatible) changes are introduced in the XML schemas**. 

Examples of these backwards compatible changes include e.g. adding optional properties to existing types or adding new types.

Existing data valid according to the older schema will also remain valid according to the newer schema.

* **'Z' is the bugfix version number - Updates of this number** (e.g. 3.0 --> 3.0.1) **are applied when errors or bugs are fixed in the XML schemas**. Although bug-fixes are often breaking (i.e. non-backwards-compatible) changes, they could also correspond to non-breaking (i.e. backwards-compatible) changes.

Examples of breaking bug-fixes include e.g. restrictions in cardinality of existing properties, adding mandatory associations to schema elements or changing the types assigned to schema elements. Examples of non-breaking bug-fixes include e.g. adding missing types or definitions to elements already defined in a schema.

Existing data valid according to the older schema will only remain valid according to the newer schema in case of non-breaking bug-fixes. Otherwise te data will no longer be valid according to the newer schema.

### How long can the deprecated schemas still be used? 

Use of deprecated schemas is discouraged. XML schemas newly endorsed by MIG should therefore be adopted by INSPIRE data and services providers within the shortest possible period of time, since the whole set of endorsed schemas constitute the basis for ensuring conformance to the requirements defined in the INSPIRE Technical Guidelines using the [INSPIRE Reference Validator](https://inspire.ec.europa.eu/validator).

Based on feedback from MIG-T, the following indicative time periods are agreed for adopting any newly endorsed XML schemas: 

* Deprecated versions should no longer be used after 2 years after a major release (corresponding to changes in the major version number).

* Deprecated versions should no longer be used after 1 year after a bugfix release (corresponding to changes in the bugfix version number).

* There should not be specific deadlines for minor releases (corresponding to changes in the minor version number), i.e. the deprecated minor version can still be used as long as the corresponding major version may be used. 

It should be noted that, since the schemas are not legally required, the periods indicated above only constitute recommendations.

## INSPIRE draft XML schema repository

### Location, Structure & Content of the repository

**An additional repository is available at https://inspire.ec.europa.eu/draft-schemas which contains extended data models included in the Technical Guidelines**.

The structure used within this repository of draft XML schemas follows the same structure of folders and sub-folders and versioning rules explained above for the [official repository of INSPIRE XML schemas](https://inspire.ec.europa.eu/schemas).
