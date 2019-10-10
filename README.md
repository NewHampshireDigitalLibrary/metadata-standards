# New Hampshire Digital Library Metadata Standards
## A Simple Guide to Describing Your Digital Objects

Any item that is intended to be shared online should have descriptive information associated with it. This information is called metadata, or, “data about data.”

It is important to write metadata in a manner that is consistent with established standards. This consistency helps computer systems present the information correctly on the screen, and also enables the ability to search and browse resources from several institutions all at one time. Without consistent, quality metadata, this would be very difficult.

In December 2017, the Digital Public Library of America (DPLA) published version 5.0 of the Metadata Application Profile, available from https://pro.dp.la/hubs/metadata-application-profile. The profile provides guidance for writing metadata in a manner that is both consistent with other institutions and allows those institutions to easily share their resources on the DPLA platform.

This document is a simplified guide for writing metadata according to those DPLA specifications.



## General guidelines <sup>[1](#footnote1)</sup>

### Avoid abbreviations
Avoid the use of abbreviations. Spell out the full names of communities and states. For example, use “Mount Washington,” not “Mt. Washington” and “New Hampshire,” not “NH.” 

Exceptions where the use of abbreviations is acceptable include terms used with dates (such as “b.” for “born”), distinguishing terms added to names of persons (such as "Mrs."), or widely accepted terms (such as “St.” for “Saint”), or abbreviations prescribed by controlled vocabularies for use in the Subject field (e.g. “Beloit (Wis.)” from Library of Congress Subject Headings).

### Capitalization
Capitalize all proper names. Capitalize only the first word in titles and subject terms. Capitalize content in the description field according to normal rules of writing. Do not enter content in all capital letters except in the case of acronyms.

### Characters to avoid
Do not use ampersands (&) or ellipses (. . .). Do not use HTML tags. For example, do not use `<br>` or `<br />` within metadata fields to force a line break.

### Unknown data
Fields for which there is no available information should be left blank. Avoid using “unknown,” “anonymous,” etc.

---
Metadata describing each item is written according to the Dublin Core Qualified metadata schema. While there are many Dublin Core elements, the following are either required or recommended.

Guidelines for filling in the following metadata elements are described in this document:

|Field Name|Dublin Core Element| Required by DPLA| Required by NH HUB|
|----------|-------------------|-----------------|-------------------|
|Creator |dc.creator| Strongly Recommended|Strongly Recommended|
|Contributor |dc.contributor| Optional|Optional|
|Date |dc.date |Strongly Recommended|Strongly Recommended|
|Description |dc.description |Strongly Recommended|Strongly Recommended|
|Format |dc.format |Optional|Optional|
|Identifier |dc.identifier |Optional|Required
|Language |dc.language |Required|Required|
|Location |dc.coverage |Strongly Recommended|Strongly Recommended|
|Physical Repository |dc.provenance |Required|Required|
|Publisher |dc.publisher |Optional|Optional|
|Rights |dc.rights |Required|Required|
|Subject |dc.subject |Strongly Recommended|Strongly Recommended|
|Title |dc.title |Required|Required|
|Type |dc.type |Required|Required|

## Guidelines for using the elements
When describing an object, describe the physical resource.

### Required Elements

#### Identifier
An unambiguous reference to the resource. Recommended best practice is to identify the resource by means of a string conforming to a formal identification system.

For example, a collection from the Nashua Public Library might be numbered thus:
NPL201700001; NPL201700002; NPL201700003; etc.
Where NPL stands for Nashua Public Library; 2017 represents the year it was digitized, and 00001 is the number of the individual item.

Each institution may create their own identifying system, but they must be consistent and unique.

#### Language
Required when the object contains readable text. Use the ISO 639-2 code. 

For example:
English: eng
French: fre
Greek: gre
Latin: lat
Spanish: spa

For other language codes, please see: 
https://www.loc.gov/standards/iso639-2/php/code_list.php

#### Rights
Statement describing the copyright status or other rights and restrictions associated with the resource. 

Select the appropriate statement from [RightsStatements.org](http://rightsstatements.org/en/). Examples:

|Rights Statement |RightsStatements.org Definition|
|-----------------|-------------------------------|
|http://rightsstatements.org/vocab/NoC-US/1.0/ |**No Copyright** - United States. This Rights Statement should be used for Items for which the provider has determined are free of copyright under the laws of the United States. This Rights Statement should not be used for Orphan Works (which are assumed to be in-copyright) or for Works where the data provider has not undertaken an effort to ascertain the copyright status of the Work.|
|http://rightsstatements.org/vocab/InC-RUU/1.0/ |**In Copyright - Rights-Holder(s) Unlocatable Or Unidentifiable.** This Rights Statement is intended for use with an Item that has been identified as in copyright but for which no rights-holder(s) has been identified or located after some reasonable investigation. This Rights Statement should only be used if the data provider is reasonably sure that the work is in copyright.|
|http://rightsstatements.org/vocab/InC-EDU/1.0/ |**In Copyright - Educational Use Permitted.**  This Rights Statement can be used only for copyrighted Items for which the organization making the Item available is the rights-holder or has been explicitly authorized by the rights-holder(s) to allow third parties to use the Work for educational purposes without first obtaining permission.|
|http://rightsstatements.org/vocab/InC/1.0/ |**In Copyright.** This Rights Statement can be used for an Item that is in copyright. Using this statement implies that the organization making this Item available has determined that the Item is in copyright and either is the rights-holder, has obtained permission from the rights-holder(s) to make the Work available, or makes the Work available under an exception or limitation to copyright (including Fair Use) that entitles it to make the Work available.|


#### Title
When it is a published item (like a book or map):
Enter the title exactly as it is written on the object. Only capitalize the first word and any proper nouns.

When it is an unpublished item (like a photograph or letter):
* Look for a title from the creator, such as a caption.
* If this does not exist, write your own title. Include the creator of the item (if known) and the subject matter in the title, particularly the location if known.

#### Type
A term broadly characterizing the type of resource being described.

Select the appropriate term from the DCMI Type vocabulary: http://dublincore.org/documents/2010/10/11/dcmi-type-vocabulary/

|Example |Definition|
|--------|----------|
|MovingImage |A visual representation in motion, such as movies, television programs, animation|
|Sound |A resource primarily intended to be heard, such as oral history audio recordings, music|
|StillImage |A static visual representation other than text, such as photographs, postcards, maps, paintings, and images of three-dimensional objects|
|Text |A resource consisting primarily of words for reading, such as books, articles, letters, diaries, yearbooks, or manuscripts|


### Strongly Recommended Elements

#### Creator
The person or organization responsible for creating the item, such as an author or photographer. 

If a personal name, enter in Lastname, Firstname format.

#### Date
The date the item was either created or published. Use the format YYYY-MM-DD, YYYY-MM, or YYYY for a single known date.

|Example |Explanation|
|--------|-----------|
|1927 |Date of a postcard with the year 1927 printed on it|
|1927-07 |Date of a painting created in July 1927|
|1927-07-03 |Date of a photograph taken on July 3, 1927|
|ca. 1927| Map likely created in 1927 or close to it|
|1910-1920 |Photograph created between 1910 and 1920|

#### Description
A free-text description of the resource. 

The description should be written in complete sentences. Do not use abbreviations, ampersands or paragraph and line breaks. Maintain standard capitalization rules.

#### Location
The location or area that is described or represented by the resource. 

Enter the most specific element of the location known (e.g. city, village) followed by the state name. Avoid abbreviations. Use of the Getty Thesaurus of Geographic Names (TGN) is encouraged.

Examples: 
- New Hampshire
- Concord, New Hampshire
- Dianas Baths, Carroll County, New Hampshire
- Mount Chocorua, Carroll County, New Hampshire

#### Subject
Topic of described resource. Generally, this field will contain terms that describe what is depicted in an image, or terms that describe what a text is about.

Use of a controlled vocabulary such as:
Library of Congress Thesaurus for Graphic Materials (LCTGM): http://id.loc.gov/vocabulary/graphicMaterials.html

Getty Art and Architecture Thesaurus (AAT)
http://www.getty.edu/research/tools/vocabularies/tgn/

Nomenclature 4.0
http://resource.aaslh.org/view/nomenclature-4-0-for-museum-cataloging/

For multi-word subject terms, capitalize just the first word, unless other words are proper nouns. Enter multiple subject terms in separate fields.

### Optional Elements

#### Contributor
A person or organization who contributed to creating the resource. For example, an illustrator of a book, or a curator of a collection. If a personal name, enter in Lastname, Firstname format.

#### Format
A description of the physical manifestation of the resource. Terms are drawn from the Art & Architecture Thesaurus (http://www.getty.edu/research/tools/vocabularies/aat/index.html)

#### Publisher
Name of the person, organization, or service responsible for publishing the original resource. Publishers can be a corporate body, museum, historical society, university, etc.

This field may also contain the place of publication in addition to the publisher name. If including the place of publication, enter as "Location: Publisher name.”

Example: Concord, New Hampshire: New Hampshire Historical Society

Questions?
Contact the New Hampshire DPLA Hub Metadata Committee:
[NH-digital-library-tech@googlegroups.com](mailto:NH-digital-library-tech@googlegroups.com)

<a name='footnote1'>1</a>: Credit for this section goes to Recollection Wisconsin Metadata Essentials, November 2016
