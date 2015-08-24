<!---

BIBFRAME Archive is a starting point for archival vocabularies using the 
http://bibfra.me model and profiles. It builds off of the BIBFRAME Lite vocabulary. 
It is framework conformant to BIBFRAME and . and where possible, link-compatible with the 
US Library of Congress's BIBFRAME vocabulary, http://bibframe.org/

BIBFRAME Archive is expressed using the Versa data model, which also
allows for full expression in RDF form.  This particular file is in
the Versa Literate syntax, based on the Markdown format
<https://daringfireball.net/projects/markdown/basics>.

The convention for expressing data models in Versa Literate has each
vocabulary item starting with a new header, A level 1 header for
resource classes and level 2 for properties.  Each has its ID as an
IRI reference (usually relative). Each is then described within its
section's unordered list, given a "label" (display label),
"description" (also for explanatory display), possibly "synonyms" (one
or more loose expression that the resource can be considered a synonym
for another). Resource classes may also have "properties"
(space-separated list of property IDs defined on the
resource). Properties may also have "value" (textual description of
the expected value of the property, perhaps as a relationship to
another resource, or as a data value).

You'll notice that BIBFRAME Archive terms use a humpCase/HumpCase convention,
which derives from BIBFRAME legacy.

-->

# @docheader

<!---

@base is the default base IRI, used e.g. for resource headers. It
would also be used for properties except that it is overridden by
@property-base

The meta-properties in this file are actually defined by the Versa
data model to support interpretation by Versa modeling tools

@resource-base is another possible override, for resource headers, but
not used here

-->

* @iri:
    * @base: http://bibfra.me/vocab/archive/
    * @property: http://bibfra.me/purl/versa/support
* title: BIBFRAME Archive vocabulary
* @interpretations:
    * scope: @resource

<!---
Extend BIBFRAME Lite Classess
--->

# <http://bibfra.me/vocab/lite/Work>
* properties:  

# <http://bibfra.me/vocab/lite/Instance>
* properties: 

# <http://bibfra.me/vocab/lite/Authority>

# <http://bibfra.me/vocab/lite/Person>
* properties: 

# <http://bibfra.me/vocab/lite/Organization>
* properties: 

# <http://bibfra.me/vocab/lite/Meeting>
* properties: 

# <http://bibfra.me/vocab/lite/Topic>
* properties: 

# <http://bibfra.me/vocab/lite/Form>
* properties: 

<!---

Class Refinements 
-->


# findingAid

* label: finding aid
* refines: <http://bibfra.me/vocab/lite/findingAid>
* synonyms: 
* description: A work with finding aid characteristics that describes archival collections to give the repository physical and intellectual control over the materials, and assist users in gaining access to and understanding the materials
* value: Literal
* properties: eadId 
* scope: <http://bibfra.me/vocab/archive>
* remark: 

<!---

Properties - [Terms below are mapped from Structural and Other Limited EAD Elements]

-->

## eadId

* label: EAD Identifier
* refines: <http://bibfra.me/vocab/lite/controlCode>
* synonyms: 
* description: Designates a unique code for a particular EAD finding aid document
* value: Literal
* scope: <http://bibfra.me/vocab/archive>
* remark: Equivalent to EAD ID <eadid>

<!---

EAD elements below are not mapped to the terms above: 

<ead> – EAD wrapper
<eadheader> – EAD Header
<filedesc> –  File Description 

-->

<!---

List of EAD3 Elements: 

abbr
abstract
accessrestrict
accruals
acqinfo
address
addressline
agencycode
agencyname
agent
agenttype
altformavail
appraisal
archdesc
archref
arrangement
author
bibliography
bibref
bioghist
blockquote
c
c01
c02
c03
c04
c05
c06
c07
c08
c09
c10
c11
c12
chronitem
chronitemset
chronlist
citation
colspec
container
control
controlaccess
controlnote
conventiondeclaration
corpname
custodhist
dao
daoset
date
daterange
dateset
datesingle
defitem
descriptivenote
did
didnote
dimensions
dsc
ead
edition
editionstmt
emph
entry
event
eventdatetime
eventdescription
eventtype
expan
famname
filedesc
fileplan
footnote
foreign
fromdate
function
genreform
geogname
geographiccoordinates
head
head01
head02
head03
index
indexentry
item
label
langmaterial
language
languagedeclaration
languageset
lb
legalstatus
list
listhead
localcontrol
localtypedeclaration
maintenanceagency
maintenanceevent
maintenancehistory
maintenancestatus
materialspec
name
namegrp
notestmt
num
occupation
odd
originalsloc
origination
otheragencycode
otherfindaid
otherrecordid
p
part
persname
physdesc
physdescset
physdescstructured
physfacet
physloc
phystech
prefercite
processinfo
ptr
ptrgrp
publicationstatus
publicationstmt
publisher
quantity
quote
recordid
ref
relatedmaterial
relation
relationentry
relations
repository
representation
row
scopecontent
script
separatedmaterial
seriesstmt
source
sourceentry
sources
sponsor
subject
subtitle
table
tbody
term
tgroup
thead
title
titleproper
titlestmt
todate
unitdate
unitdatestructured
unitid
unittitle
unittype
userestrict

-->
