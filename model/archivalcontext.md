<!---

BIBFRAME EAC-CPF is a starting point for archival vocabularies using the 
http://bibfra.me model and profiles. It builds off of the BIBFRAME Lite vocabulary 
and Encoded Archival Context—Corporate Bodies, Persons, and Families (EAC-CPF).
It is framework conformant to BIBFRAME and where possible, link-compatible 
with the Library of Congress's BIBFRAME vocabulary, http://bibframe.org/

BIBFRAME context is expressed using the Versa data model, which also
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

template 

# lowerCase/UpperCase

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark: 

--> 

<!---

For definitions see: http://eac.staatsbibliothek-berlin.de/fileadmin/user_upload/schema/cpfTagLibrary.html

Elements

abbreviation   abstract   address   addressLine   agencyCode   agencyName   
agent   agentType   alternativeForm   alternativeSet   authorizedForm   biogHist   
chronItem   chronList   citation   componentEntry   control   conventionDeclaration   
cpfDescription   cpfRelation   date   dateRange   dateSet   description   descriptiveNote   
eac-cpf   entityId   entityType   event   eventDateTime   eventDescription   eventType   
existDates   fromDate   function   functionRelation   functions   generalContext   identity   
item   language   languageDeclaration   languagesUsed   languageUsed   legalStatus   legalStatuses   
level   list   localControl   localDescription   localDescriptions   localTypeDeclaration   
maintenanceAgency   maintenanceEvent   maintenanceHistory   maintenanceStatus   mandate   
mandates   multipleIdentities   nameEntry   nameEntryParallel   objectBinWrap   objectXMLWrap   
occupation   occupations   otherAgencyCode   otherRecordId   outline   p   part   place   
placeEntry   placeRole   places   preferredForm   publicationStatus   recordId   relationEntry   
relations   resourceRelation   script   setComponent   source   sourceEntry   sources   span   
structureOrGenealogy   term   toDate   useDates  

Attributes

accuracy   altitude   countryCode   cpfRelationType   functionRelationType   
identityType   languageCode   lastDateTimeVerified   latitude   localType   longitude   
notAfter   notBefore   resourceRelationType   scriptCode   standardDate   standardDateTime   
style   transliteration   vocabularySource   xlink:actuate   xlink:arcrole   xlink:href   
xlink:role   xlink:show   xlink:title   xlink:type   xml:base   xml:id   xml:lang 

--> 
