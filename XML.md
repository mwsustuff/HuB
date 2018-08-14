

we want a simple application just to store the data and further make it availalbe for our business application.

* GML(Gneralized MarkupLanguage)------>ibm

* SGML--->standard Generalized Markup Language

#### w3c(WorldWidewebConstorism..)

In simple terms sgml is used to define markup language
ex: Html(HyperTextmarkupLanguage) is one of the markup language derived from sgml


__XML----->(extensible MarkUpLanguage)__

is a meta markup language used to define a markup language.
some of the markup languages dervied the xml standards are

* xhtml
* wml
* vml
* mathMl
* cml

note: html is a simple markup language derived from sgml where as xml is a meta markup language which is used to define markup langagues like html

what is the difference between html and xml?
html
=====
predefined taga
limited no of tags
Tags are case insensitive
tags are meant for displaying the data but not for descbing the data
html focuses on how data looks

xml
====
user defined tags
tags are extedsnsible
tags are case senstive
tags are meant for describing the data
xml focuses on waht data is....

what is purpose of xml
==============================
xml is used to exchange the information between application in language(java,.net.php) independent
vendor indepednent and platform independent manner over web.

xml documents are used to testual databases
xml documents are sued as deployment descriptors
xml is used to Create new internet languages (xhtml,wsdl,wap,smil.....)


XML(dtd,xsd)
===========
To persist the data
complexty of the application was increased
increaed the development time and cost of the application
it was more error prone
As the data format prepared was not generic,future extensions were becoming difficult

ex:DBMS,MessageServer,MailServer..............

IBM---> GmL(Generalized MarkUp Language)
SGML-->Standard Generalized Markup Language
w3c

In Simple Terms SGML is used to define a markup language

ex: Html(Hyper TExt Markup Language) is one of the markup language derived from SGML

MarkUpLanguage
================

XML(Extensible Markup Language)is a meta markup language used to define a markup language

Some of the markup languages derived the xml statndards 
Xhtml(extensible hypertextmarkup language)
wml(wireless markup language)
mathMl(mathematical markup language)
cml-->chemical markup language
vml-->vector markup language

note: html is a simple markup language derived from sgml where as xml is a meta markup language which is used to define markup languages like html
xml standards are given and managed by w3c
uses of xml(markup language)
=============================
1)markup language is used as temporary data store or a minidata store-->bcz of the 
self descriptive
simpletext format

2) it is used to transfer data from one appliction to another we use this
self descriptive
supports unicode standars --> xml documnet can be written any encoding format wich are given under unicode standards.
wide support from almost all the enviornments

3) It is used to describe some information or give instructions to an application or product
self descriptive which makes the document to be less error prone.
what is purpose of xml
==============================
xml is used to exchange the information between application in language(java,.net.php) independent
vendor indepednent and platform independent manner over web.

xml documents are used to testual databases
xml documents are sued as deployment descriptors
xml is used to Create new internet languages (xhtml,wsdl,wap,smil.....)

q)what xml does?

Nothing!
just xml was created to strucutre,store and trasport the data


<email>
<to>shiva</to>
<from>sirisha</from>
<subject>Rminder party</subject>
<body>dont forget me this sunday</body>
</email>

but sitll this xml document does not do anything . it just information wrapped in tags.Someone must write a peice of Software
to send ,receive or display it.

<?xml version="1.0"
<email>
<to>shiva</to>
<from>sirisha</from>
<subject>Rminder party</subject>
<body>dont forget me this sunday</body>
</email>

xml elements must have a closeing tag
eg:<subject>Rminder party</subject>

xml tags are case sensitive
eg:<subject>Rminder party</subject>

xml elements must be properly nested
<b><i>this text is bold </i></b>

all xml documents must hv a root tag

Attributes values must always be quoted.
<email date="12/05/2014">
EntityReferences
========================
<message>if salary < 1000 then</message>
To aovid this error, replace the < character with an entity referece.

There are 5 Predefined entity references in xml
=================================================
<    &lt
>    &gt
&    &amp   
'    &apos
"   qotationmark
<message>if salary &lt 1000 then</message>

note: Only the characters < and & ae strictly illegal in xml.

comment in xml
<!--  this is a comment -->

White-space is preserved in xml
html Hello    shiva    hello shiva
xml  Hello    shiva    hello      shiva

q)What is well-formed xml document?
if an xml document confirms the syntactical rules of xml specification is said to be well formed

it must begin with xml delcaration
it must hv one unique root element
start tags must hv matching end tag
elemetns are case senstive
all elements must be closed
all elemnets must be propertly quoted
all attributes values must be quorted
Entities must be used for special caharacters

Q)Who invented xml tags?
q)what ia xml document?
Any text file that is developed with .xml extendsion is a an xml document.
q)What is xml application?
Any comupter application that work with an xml document is nothing but an xml application.
q)What are the xml naming rules
xml elements must 
1)names can contain letters,numbers and other characters
2)names cannot start with a number or punctation character
3)names cannot start with the letters xml(or xml,or xml,...)
4)names cannot contain spaces
Any name can be used no words are reserved...
5)Avoid : character.Colons are reserved to be used for something called namespaces.

Q) What are Best Naming Practices?
1)make names descripvie.names with an underscore separator are nice: <first_name>,<last_name>
2)names should be short and simple like this<book_title> not like this<this_title_of_the_book>
3)Avoid - charcater if you name something first-name ,software may think you want to subtract name from first
4)avoid . charactersif you name something first.name ,software may think that name is a property of the object first
5)avoid : characters colons are reserved to be used for something called namespaces...


Terminalogy
===========
xml--> This term represents the standards to design and develop a markup language
xml markp language
======================
is used to represent a markup language which is designed and developed according to xml
xml document
================
this represent a doument which is written accoring to xml and its markup language standards
To develop a markup language
==========================
step:-1
Declare the elements of the language like tags(known as elements) attributes and entitties
step-2
Define the grammar rules for the language
step-3
write an application which can put the document into action

To peform step1 and stpe2 in the markup language development under xml we hv been given with dtd and xml schema
To perform step3 develop an application (language implementation) we use parsers can be developed useing any programming language which supports xml

DTD(Doument Type Definination)
==================================
It is a part of xml standards and this part of of the specification allows us to declare the elements of our markup language and deine the grammer rules.

Inherited fromsgml provides special sytax from declaring elements attributes 
and entities

In xml all elements must hv a closing tag
<p > this is paragrap</p>
xml tags are casesensitive
xml elements must be preperoy nested
xml document must hv a root tag
attrbute values must always be quoted.


In Dtd we can declare 
1)elements
2)Attributes
3)Entities
4)Notations

Elements
============
An element (tag) is used to provide a meaning for the content which it encloses.
An element  consists of three parts
1)opentingelement
2)closing elment
3)content

eg:
<abc> hello</abc>----->element
<sal> 5000</sal>

<cinema>
<name>basha</name>
<hero>Rajanikanth</hero>
</cinema>

<name>basha</name>--->it is called one element



Element describes abut the eclosed content 
opening tag+content+closing tag=ELEMENT
<employees>
<employee></employee>
<dept></dept>
</employees>

In DTD
<!ELEMENT name of the rootelement (List of child elemnt)>
<!Element employees(employee,dept)>

eg
===
<!Element cinema(name,hero)>


Types of Elements
================
childonly
Textonly
Empty
Mixed
Any Type(This is one special type given under DTD standards and not recommanded to be used)

a)childOnly
================
This type of elements hv a content as zero or more elements
eg:
<!ELEMENT name of the lement (List of child elemnt)>
where name of element takes the element name which is being declared
eg:
===
<emp>
<name></name>
<address></address>
<sal><sal>
</emp>
<!Element emp(name,address,sal)>


for eg:
<cinema>
<name>basha</name>
<hero>Rajanikanth</hero>
</cinema>

the content of cinema is name and hero
declare child only elements as per the dtd sytax
<!Element elementname(list-of-childelements)>
<!Element cinema(name,hero)>


requriment
==============
<cinimas>
<cinema>
<name>basha</name>
<hero>Rajanikanth</hero>
</cinema>

<cinema>
<name>sarkar</name>
<hero>amitabachan</hero>
</cinema>
</cinemas>
how to declare above tag of elements useing dtd sytax

<!Elements cinemas(cinema,cinema)>


To meet the type of requirement we hv specifiers
=================================================
*---> specifies the occurance of an element is 0 or more times
+--> the  occurance of an element is 1 or more times
?--> 0 or 1 time

note: if we dont use any specifiers then default occurance of the element is considered for 1 time

<!Elements cinemas(cinema*)>

<!Elements web-app(servlet*)>



requriment
==============
<cinemas>
<cinema>
<name>sarkar</name>
<hero>amitabachan</hero>
</cinema>
<cinema>
<name>osayramulama</name>
<heroine>Vijayasanthi</hero>
</cinema>
<cinemas>
<!ELEMENT cinemas(cinema)*>
<!ELEMENT cinema(name*,(hero|heroine))*>
one more requirement
=========
<emps>
<emp>
<name></name>
<address></address>
<sal></sal>
</emp>
<emp>
<name></name>
<address></address>
<wages></wages>
</emp>

<!ELEMENT emps(name,address,(sal|wages))>

where | indicates Or


b)Textonly elements
====================
<name>sarkar123</name>
The element that contain text as content,are termed as text only elements and they are refered useing #pcdata
dtd considers the primitive types,strings all as text

sytax:
<!ELEMENT  name of thelement(#pcdata)>
<!ELEMENT  name(#pcdata)>

pcdata -->parsed character data (it is dattype in xml)
eg in xml
====
<sal> 5000</sal>
</name>hai</name>
<!Element sal (#pcdata)>
<!Element name (#pcdata)>

requriment
==============
<cinema>
<name>sarkarraj</name>
<hero>amitabachan</hero>
<heroni> </heroni>
<villan>subash</villan>
Appalama
</cinema>

<!element cinema(name,hero,heronie,villan,#pcdata)>--->invalid

c)mixedElements
The combinattion of child only and text only and empty elements we can call as mixed elements

for eg>

<cinema>
<name>sarkarraj</name>
<hero>amitabachan</hero>
<heroni> </heroni>
<villan>subash</villan>
<commedian></commedian>
xyz
</cinema>
note: for declaring mixed elements we hv a special sytax given by the dtd 
<!ELEMENT elementname(#pcdata|list of child elements separated by |)*>

<!element cinema(#pcdata Name|hero|heroni|villan|commedian)*>

eg:
===
<emp>
<name></name>
<sal></sal>
<address>
<flatno>302,srisairesidency</flatno>
ManiKonda,Hyd.
<pin>5000089</pin>
</address>
</emp>
in Dtd
=====
<!Element address (*pcdata|flatno|pin)*>

d) Empty elements
This type of element do not hold any content.
they contain  attributes which can provide an extra meaning at that position.
sytanx:
<!element elementname EMPTY>
<!element heroine Empty>
eg
===
<emp>
<name></name>
<address></address>
<sal></sal>
<working/>
</emp>
<!Element emp(name,address,sal,working?)>
<ELEMENT working empty>
e)Any elements
this type of element can be empty or it can contain any type of content.

note:

sytanx: <!ELEMENT elementname any>
now elements are completed

<cinema name="orisa" >
<name>choddi</name>
</cinema>

for eg:
<cinema language="hindi">
<name >luck</name>
</cinema>
Rules to use attributes in an element
========================================
a) attributes should appear in the root element on the start element
b)attributes consists of name and value pair 
c)attribute names should be unique
d)attributes vlaues should be ' or "
e) we can hv more then one attribute declared in an element
f)element name and attribute name should be separated useing a space character
g) the attribute name and attrbiute value are separated useing delimeter =

sytanx: <!ATTLIST elementname attributename type specifier[defaultvalue]>

specifiers
===================
1)#required specifies attribute is mandatory
2)#impled specifies attribute is optional
3)#fixed   specifies same like final in java (constant)

Different type of attributes
================================
1)CDATA
2)NMTOKEN
3)NMTOKENS
4)ID
5)IDREF
6)ENUM
7)ENTITY
8)ENTITIES
cdata
======
for eg: 
<cinema script="hello123 how are u ready to take 123 action"/>
to referes to unparsed character data where cdata allows all the character even space character and numbers also
but doesnot allow special characters like mark up language characters.
InDTd
=====
<!ATTLIST cinema script cdata/>

nmtoken
=================
<blackbook authour="shivashankar">
Referes to named token it is again similar to cdata but doesnt accept numbers and space characters
 ===========================
it refers to named tokens,takes one or more nmtoken values where space is the delimeter(separate)
<blackbook authou=" y shiva">

Id
===

Refered as primary key it accept unique values rules to use id type attributes
There must only one id type attriubte in an element
id type attributes should be unique
id type attribute values can contain numbers, but they shouldnt commence with a number
<cinema directorid="d77">
idref
=====
similar to Foreign key where idref takes on id type attributes value
eg
==
<cinema directorid="d77">
<cinema directorid="d88>

<cinema directorid="d99" producedId="d77">


idrefs
===============
takes one on more id type attributes values where space character is the dlemiter
for eg:
<cinema directoryId="d99" producerid="d77 d88">
siilar to one to many relation ship

enum
====
Represent list of values and to define enum types in the dtd doucment we hv a special sytan

<!Attlist elementname attributename(list of values spearate by|)"defaultvalue">

<cinema directoryId="d77" produceddId="d99"talk="hit">
<!Attlist cinema talk(hit/superhit)"hit">
Entity
====
takes one uparsed enitty name
DTD---->entities
=============
Entities as variables used to define shortcuts common text
Entity reference are references to entities
Entities can be declared internal
Entities can be declared external


syta
:
<!ENTITY entityname  "EntityValue"/>
eg:
<!Entity copyright "15@MAY2014">
xml
====
<author>&copyright</author>

External EntityDeclaration
==============================

we refere the content stored in a element file

sytax:

<!entity entityname system "filelocation">
eg:
<!Entity copyright System "http://www.baanayan.com/enities.dtd">

parameterentity


dvided two types

internal
====
sytax:
<!entity  entityname "content to be refered">

external
<!entity entityname system="filelocation">
note:these entities are not refered in the xml document

unparsed enitties
=======================
<!entity entityname declaring unparsed entitties 
<!entity entityname system "filelocatioln" ndata "notationname">

fogeg
<!notation nontatiname "info">
eg
<!notation gif "image/gif">

<!entitty shiva sytem "mylogo.gif" ndata gif>


doument <institue logo="shivatech">

a)<> starting tag
b)</>ending tag
c)</>selfendingtag
d) <? ?>processing tag


<?xml version="1.0"encoding="utf-8" standalone="yes/no"
>

<! > Instruction tag

How to Associated with a Dtd with xml?
===========================
We need to specfiy DOCTYPE declaration afte xml declaration.
inorder to associate a DTD with the xml doucment
A DTD can be declared
   inside an xml document
   Externalrefererence

Doctypes
============
if the dtd declared inside the xml file,it should be wrapped in a DOCTYPE defination with the sytax

internalDoctype
<!doctype rootelement "element-declaration">
example xml document with an interal dtd.
=============================
Book.dtd
=========
<?xml version="1.0"?>
<!DOCTYPE books[
<!Element books(book*)>
<!Element book(name,author,price)>
<!Element name(#pcdata)>
<!Element author(#pcdata)>
<!Element price(#pcdata)>
<!Attlist book bookid #required>]>

<books>
<book bookid="b1">
<name>xml</name>
<author>shiva</author>
<price>500</price>
</book>
<book bookid="2">
<name>xslt</name>
<author>raja</author>
<price>500</price>
</book>
</books>

ExternalDtdDeclaration
========================
if the dtd is declared in an external file,its should be wrapped in a DOCTYPE definination with the sytax
externaldoctype
<!docttype rootelement system "dtd" file location">

<!Element books(book*)>
<!Element book(name,author,price)>
<!Element name(#pcdata)>
<!Element author(#pcdata)>
<!Element price(#pcdata)>
<!Attlist book bookid #required>

<?xml version="1.0"?>
<!DOCTYPE BOOKS SYSTEM "book.dtd">
<books>
<book bookid="b1">
<name>xml</name>
<author>shiva</author>
<price>500</price>
</book>
<book bookid="2">
<name>xslt</name>
<author>raja</author>
<price>500</price>
</book>
</books>



<!doctype rootelement public /system "formalpulicidentifier "dtdfile url>
fpi
====
part
-/+

par2
name of the organization who has given the dtd
part3
what for dtd is given for
part4 tow letter language code en

Book.dtd
=========
<!Element books(book*)>
<!Element book(name,author,price)>
<!Element name(#pcdata)>
<!Element author(#pcdata)>
<!Element price(#pcdata)>
<!Attlist book bookid #required>
xml
====
<?xml version=1.0">
<books>
<book bookid="b1">
<name>xml</name>
<author>shiva</author>
<price>500</price>
</book>
<book bookid="2">
<name>xslt</name>
<author>raja</author>
<price>500</price>
</book>
</books>

In DtD
===========
Employees.dtd
===============
<!Element Employees(employee*,dept)>
<!Element Employee(name,sal,desig)>
<!Element name(firstname,middlename,lastname)>
<!Element firstname(#pcdata)>
<!Element middlename(#pcdata)>
<!Element lastname(#pcdata)>
<!Element sal(#pcdata)>
<!Element desig(#pcdata)>
<!Element dept(dname,desg)>
<!Element desg(#pcdata)>
<!Element dname(#pcdata)>
<!Attlist salary type(usd|InR)'Inr'>
<!Attlist employee empno >
<!Attlist employee mgrid Idref #implied>
<!Attlist departmnet deptno id #required>
xml application
=============
<?xml version="1.0"?
<!DocType Employees System Employees.dtd">
<Employees>
<Employee empno="emp101" mgid="emp101">
<name>
<firstname>shiva</firstname>
<middlename>reddy</middlename>
<lastname>yannam</lastname>
</name>
<salary type="usd">10000</salary>
<desg> mgr</desg>
</employee>
<Employee empno="emp102" mgrid="emp101>
<name>
<firstname>shiva</firstname>
<middlename>reddy</middlename>
<lastname>yannam</lastname>
</name>
<desg> developer</desg>
</employee>
<deparment deptno="dno">
<dname>computerscience</dname>
<desc>this dpet is responsible for s/w products</desc>
</department>
</employee>
</employees>



shiva.dtd
=============
<!element cinemas(cinema*,distrubutor,copyrights)>
<!element cinema(name,hero,villan,budget)>
<!eleement name(#pcdata)>
<!element hero(#pcdata)>
<!element villan(#pcdata)>
<!element budgent(#pcdata)>
<!element distrubutor(ditname,distlocation)>
<!element disname(#pcdata)>
<!element distlocation(")>
<!element copyrights("")>
<!attlist cinema dirid id #Required>
<!Attlist cinema proid idref #implied>

<!attlist cinema talk(hit/plop)"hit">
<!attlist distriubutor distid id #required>
<!entity copryrights "13-sep-11">


cinema.xml
=============
<?xml version="1.0"?>
<!doctype cinemas System "shiva.dtd">
<cinemas>
<cinema dirid="d77" proid=d88" talk="hit">
<name>Rangdebasaenti"</name>
<hero>amirkhan</hero>
<villan>anupamkhar</villan>
</cinema>
<copryrights>&copyrights</copyrights>
</cinemas>
======================================================================
message.xml
============
<message>
<to>shiva</to>
<from>raja</from>
<body>hi how are u</body>
<age>30</age>
</message>

message.dtd
===========
<!Element message(to,from,body,age)>
<!Element to(#pcdata)>
<!Element from(#pcdata)>
<!Element body(#pcdata)>
<!Element age(#pcdata)>

Develop an external dtd for the xml dcoument?
student.xml
===========
<?xml version="1.0"?>
<!Doctype students System "student.dtd">
<students>
<student regno="nit001">
<name>shiva</name>
<course>xml</course>
<fees-status>Notyet</fees-status>
<working>yes</working>
</student>
<student regno="nit002">
<name>sirisha</name>
<course>spring</course>
<fees-status>paid</fees-status>
</student>
</students>
student.dtd
========
<!Element students(student,faculty)>
<!Element student(name,course,fees-status,working?)>
<!Element name(#pcdata)>
<!Element course(#pcdata)>
<!Element fees-status(#pcdata)>
<!Element working(#pcdata)>
<!Attlist student regno id  #required>

items.xml
=========
<?xml version=1.0"?>
<!Doctype items System "items.dtd">
<items>
<item>
<item code="1001">
<price>2500.00</price>
</item>
<item code="1002">
<price>250.00</price>
</item>
</items>
items.dtd
=======
<!Element items(item+)>
<!Element item(price)>
<!Element price(#pcdata)>
<!Attlist item code Id  #Required>

now am provding dtd.
==================
<!Element bookstore(name,topic+)>
<!Element name(#pcdata)>
<!Element topic(topic-name,book+)>
<!Element topic-name(#pcdata)>
<!Element book(title,author)>
<!Element author (#pcdata)>
<!Element tile (#pcdata)>
<!Attlist book isbn Id  #Required>

bookstore.xml
============
<?xml version="1.0"?>
<!DocType bookstore system "bookstore.dtd">
<bookstore>
<name>HydBookstore</name>
<topic>
<topic-name>xml</topic-name>
<book isbn="b12" color="red" pages="150" publiccation="MCGRill">
<title>dtd and xml schemas</title>
<author>shiva</author>
<price>50</price>
</book>
<book isbn="b123">
<title>xsd in 24 hurs</title>
<author>shiva</author>
</book>
</topic>
</bookstore>


What do you know about SYSTEM keyword in DOCTYPE declaration
System keyword indicates that the specified dtd is private one. Almost always we use this
(System) keyword only in Doctype dec
Another keyword is alternative for System is PUblic


eg:
===
<!Doctype web-app public "-//sumicrosystems,inc//DTD webAppication 2.5 //en" "http://java.sun.com/j2ee/dtds/web-app 2 5.dtd">

+ --->Standardized body
-  --->non-standardized body
w3c=organziation name
en=english
verions 2.5 =versionaname

DTD limitations
=============
cannot define our own data types
doesnt support namespaces

Xsd
=============
can define our own data types
supports namespace


===========================================================================================

WebServices
============
Requirement
============
We need to integrate some set of Objects Which are running and developed in Different platForm to build into our System.


WebSevices is a Distibuted Technology Acieves Interoperability(Portablity across different Technologies such as Java,.Net,PHP,C,C++......)

The Other Distributed Technologies like Corba,RMi,Ejb,Dcom,C++ ....Uses Binary Format,hence the objects are Serialized into Stream of Bytes.

WebServices uses Xml Format Instead of Binary Format,Hence the webservices the data is exchanged as xml message,which is validated against xml schema(xsd) but not DTD,Since xsd additionally supports data types.In Webservices The objects are Serialized into xml message.

The WebServices Technologies such as SoAp,WSDL,UDDI are represented in xml against corresponding SChemas.


XmlSchemaDefinition(XSD)
==========================
Xml Schema Describes the structure of Xml Document
The xml schema language is also called as xml schema Definition(xsd)

An Xml Schema
==============
1)Defines elements that can appear in a Document
2)Deines attribute that can appear in a Document
3)Defines Data Types For elements and attributes
4)Defines child elements and their hierarchy
5)Defines the number of child elements and their sequence
6)Defines whether an element is empty or can include text
7)Defines default and fixed values for elements and attributes.

Xml Schemas are richer and powerfull than DTD
1)Xml schemas are extensible to future additions
2)Xml Schemas Themselves are written in XMl
3)Xml shemas support data types
4)xml schemas support namespaces(it contains xml types and xml elements)


Xml Schemas are Extensible
==========================
Xml Schemas are Extensible bcz They are written in xml

with an Extensible scema definition we can
a)Reuse our schema in other schemas
b)Create our own data types derived from the standard types(simple types)
c)Referece multiple schemas in the same document.

DataTypes
=============
One of the Greatest Strength of Xml schema is the support for data types.By useing DataTypes.
a)Describes allowable document content.
b)validate the correctness of data
c)Work with data from a database
d)Define data facets(restriction on data)
e)Define data patterns(Data Formats)

Xml Data Types are
1)SimpleTypes
2)ComplexTypes

1)SimpleTypes
================
The xml element is defined useing simple types and contains only text without attributes or subelements all Built-in-types(Both primitive and Derived types)are simple Types.

Built-in type with Restrictions are also simple types.

xml schema specified 44 built in types

Built-In Types are
=================
1)primitive types
eg: 
string 
boolean
decimal
float
double
druation
dattime
time
date
gyearmonth
qname
notation
----


2)Built-in Derved types.
Integer
Long
Short
Byte
NOnPositiveINteger
---
--NmTokens
NmToken
id
idref
idrefs
entity
entities

The most Common types are
=================
xs:String
xs:decimal
xs:integer
xs:boolean
xs:date
xs:time

Define Simple Elements
=========================
simple xml elements are defied useing simple types.
sytax:
<xs:element name="element-name" type="element-type"/>
eg:
<xs:element name="firstName" type="xs:string"/>
where element-name is the name of the element and element -type is the data type of the element.
what is the xsd equivalent for the xml element
xmlelements
<lastname>yannam</lastname>
<age>30</age>
<dateborn>1982-01-14</dateborn>
xsd definations
=============
<xs:element name="lastname" type="xs:string"/>
<xs:element name="age" type="xs:integer"/>
<xs:element name="dateborn" type="xs:date"/>

How to give default and fixed values to simple element
"color" element default value is red
<xs:element name="color" type="xs:String" default="red"/>

"color" element fixed value is yellow
<xs:element name="color" type="xs:String" fixed="yellow"/>
how to define an Attribute?
sytax:
=====
<xs:attribute name="attribute-name" type="attribute-type"/>

xml element
========
<lastname lang="En">yannam</lastname>
xsd defination
============
shiva.xsd
========
<xs:attribute name="lang" type="xs:string"/>
<xs:element name="lastname" type="xs:String"/>

how to define fixed and default values to attributes

fixed values for Attributes
<xs:attribute name="lang" type="xs:string" fixed="En"/>

default values for attributes
<xs:attribute name="lang" type="xs:string" default="En"/>

how to specify an attributes as optional/required?

optional attributes
<xs:attribute name="lang" type="xs:string"/>
note: By default an attribute is optional attribute

Required Attribute
<xs:attribute name="lang" type="xs:string" use="required/>

XSD Restrictions/Facets
==================
Built-intypes with Restrictions
==================================
Built-in types with restrictions are simpletypes Restrictions are used to define acceptable values for xml elements or attributes.Restrictions on xml elements are called facets.

Restrictions for DataTypes
====================
Enumeration
Length
maxExclusive
maxInclusive
maxLength
minExcclusive
minInclusive
pattern
totalDigits
whiteSapce
note: To apply above restriction to the elements are attributes we need to use
<xs:restriction> and <xs:simpletype> include <xs:element> or <xs:attribute>

Restriction on Values
======================
define element name is called age with a restriction The value of the age cannot be lower than 18 or greater than 30
<xs:element name="age">
<xs:simpletype>
<xs:restriction base="xs:integer">
<xs:minExclusive value="18"/>
<xs:maxinclusive value="30"/>
</xs:restriction>
</xs:simpletype>
</xs:element>
Restriction on Set of Values
================================
To limit the content of an xml element to a set of acceptable values, we would use the enumeration constraint.
<xs:element name="car">
<xs:simpleType>
<xs:restriction base="xs:String">
<xs:enumeration value="Audi"/>
<xs:enumeration value="Golf"/>
<xs:enumeration value="Bmw"/>
</xs:restriction>
</xs:simpletype>
</xs:element>

same eg taking the support userdefined datatype
<xs:element name="car" type="carType">

<xs:simpleType name="carType">
<xs:restriction base="xs:String">
<xs:enumeration value="Audi"/>
<xs:enumeration value="Golf"/>
<xs:enumeration value="Bmw"/>
</xs:restriction>
</xs:simpletype>
</xs:element>

Restriction on Series of Values
================================
The 'pattern' constraint is used to limit the content of xml element define a serious of numbers or letters.
eg
===
The only Acceptable value is one of the Lowercase letters from a to z
<xs:element name="letter"
<xs:simpleType>
<xs:restriction base="xs:string">
<xs:pattern value="[a-z 0-9 A-Z]"/>
</xs:restriction>
</xs:simpleType>
</xs:element>
eg1
=================
Acceptable value is Three of Uppercase letters from a to z
<xs:element name="initlas">
<xs:simpleType>
<xs:restriction base="xs:string">
<xs:pattern value="[a-z A-Z][a-z A-Z][a-z A-Z]"/>
</xs:restriction>
</xs:simpletype>
</xs:element>

ex-2
=========
The acceptable value is zero or more occrences of lowercase letters from a to z.

<xs:simpleType>
<xs:restriction base="xs:string">
<xs:pattern value="([a-z]*"/>
</xs:restriction>
</xs:simpletype>
ex-3
======
The only acceptable value is male or female
<xs:element name="gender">
<xs:simpleType>
<xs:restriction base="xs:string">
<xs:pattern value="male|female"/>
</xs:restriction>
</xs:simpletype>
</xs:element>
eg-4
===
Accepable value is five digits in a sequence and each digit must be in a range from 0 to 9
<xs:element name="prodid">
<xs:simpleType>
<xs:restriction base="xs:integer">
<xs:pattern value="[0-9]"/>
</xs:restriction>
</xs:simpletype>
</xs:element>
Restrictions on WhiteSpace characters
<xs:element name="address">
<xs:simpleType>
<xs:restriction base="xs:string">
<xs:whiteSpace value="preserve"/>
</xs:restriction>
</xs:simpletype>
</xs:element>
note: The whiteSpace constraint is set to preserve it means that xml processor will not remove any white space character.
replace  -->all tabs,line feeds returns are replaced by single spaces.
collapse-->all tabs ,linefeeds replaced by single space then all groups of single spaces are replaced with one singe space.
Restrictions on Length
=========================
To limit the length of a value in an element we would use the length,maxLength,and minLength constraints.

eg-1
==================
Define element called password with a restriction The value must be exactly eight characters.
<xs:element name="password">
<xs:simpleType>
<xs:restriction base="xs:string">
<xs:length value="8"/>
</xs:restriction>
</xs:simpletype>
</xs:element>

eg:-2
=========
difine element called password with a restriction the value must be minimum 5 characters and maxmimu 8 characters.
<xs:element name="password">
<xs:simpleType>
<xs:restriction base="xs:string">
<xs:minlength value="5"/>
<xs:maxlength value="8"/>
</xs:restriction>
</xs:simpletype>
</xs:element>
============================================================================================================================================================================
Attributes related to Restrictions
====================================
enumeration defines a list of Acceptable values
maxLength must be equal or greather than zero
minLength must be equal to or greater than zero
maxExclusive 
minExclusive
MaxInclusive
minExclusive
Pattern
TotalDigits
Length


ComplexTypes
================
The xml elements is defined useing complex type and contains Text, attributes ,subelements or both.
complexTypes are defined useing<complexType>element
eg:
=========
Define fullname of a person

<xs:complexType  name="fullNameType">
<xs:sequence>
<xs:element name="firstname" type="xs:string"/>
<xs:element name="lasttname" type="xs:string"/>
</xs:sequence>
</xs:complexType>
xml
====
<firstname></fristname>
<lastname</lastname>
note: it is not nessary to explicity declare that a simple-type element is a  simpletype. it is necessary to specify that a complex-type element is a complex type.This is done with the xs:complexType element.

How to define a Complex Element
==========================
ComplexTypes are defined useing<complexType> in two approaches

approach -1
The person element can be declared directly by nameing the element

<xs:element name="person">
<xs:complexType>
<xs:sequence>
<xs:element name="name" type="xs:string"/>
<xs:element name="age" type="xs:integer"/>
</xs:sequence>
</xs:complexType>
<sequenc> indicator. this means that the child elements must appear in the same order as they are declared.
<person>
<name>shiva</name>
<age>30</age>
</person>



Approach-2
the person element can hv a type attribute that referes to the name of the complex type
<xs:element name="person" type=personType>
<xs:complexType name="personType">
<xs:sequence>
<xs:element name="name" type="xs:string"/>
<xs:element name="age" type="xs:integer"/>
</xs:sequence>
</xs:complexType>
note: advantage os this approach is several elements can refer the same complex type.

eg
<xs:element name="employee" type="PersonType"/>
<xs:element name="student" type="PersonType"/>
<xs:element name="member" type="PersonType"/>


Define Complex Elements
=======================
There are four types of Complex Elements
1)Element with Attributes
2)Element with subElements
3)Element with attributes and text
4)Element with subElements and text

Default Automatically Assigned when no value specified explictly
Fixed   Automatically assigned and we cannot specify another value 
Use     indicates whether attribute is optioal or mandaory use="required"

1)Element with Attributes
An empty complex element cannot hv contents,only attributes
<xs:element name="product">
<xs:complexType>
<xs:attribute name="proid" type="xs:positiveInteger"/>
<xs:complexType>
</xs:element>
<product proid="123"></product>
it is possible to declare the product element like this...

<xs:element namae="product">
<xs:complexType>
<xs:complexContent>
<xs:restriction base="xs:integer">
<xs:attribute name="proid" type="xs:positiveInteger"/>
</xs:restiction
</xs:complexContent>
</xs:complexType>
</xs:element>

In the eg We define a complex type with a complex content. The complexContent element signals that we restrict or extend the content model of a complex type, and the restriction of integer declares one attibute but does not introduce any element content.

eg:
<product pid="145"/>

2)Element with Attributes and Text
=================================
It contains only text and attributes. we add a simplecontent element around the content. When useing simpleContent,we must define an extension or restriction within the simplecontent element.

<xs:element name="shoesize">
<xs:complexType>
<xs:simpleContent>
<xs:extension base="integer">
<xs:attribute name="country" type="xs:String"/>
</xs:simpleContent>
</xs:extension>
</xs:complexType>
</xs:element>

eg:
<shoesize country="france">35</sohesize>


Elements With SubElements
==========================
you can define the "person" element in a schema,
<xs:element nmae="person">
<xs:complexType>
<xs:sequence>
<xs:element name="firstname"type="xs:string"/>
<xs:element name="lastname"type="xs:string"/>
</xs:sequence>
</xs:complexType>
</xs:element>

eg:
====
<person>
<firstname>shiva</firstname>
<lastname>yannam</lastname>
</person>

Elements With SubElements and Text
===================================
An xml element contains both text and sub elements
<xs:element name="employee" type="letter">
<xs:complexType mixed="true">
<xs:sequence>
<xs:element name="name"type="xs:string"/>
<xs:element name="shipdate"type="xs:Date"/>
<xs:element name="orderid"type="xs:positiveInteger"/>
</xs:sequence>
</xs:complexType>
</xs:element>


eg:
<letter>
Dear Mr:<name>shiva</name>
Your order <orderid>111</orderid>
will be shipped on<shipdate>27-02-20012</shipdate>
</letter>
Empty Elements
==================
an empty element is an element that contains no cotent but it may hv attributes The Homepage elemnt in the instance document is an empty element
<HomePage url="http:www.martwain.com"/>
indicators
==============
we can control how eleements are to be used in documents with indicators.
1)All
2)Choice
3)sequence
Occurance Indicators
1)MaxOccurs
2)MinOccurs
Group indicators
GroupName
AttributeGroup name

All
===
<all> indicator specifies the child elements can appear in any order, and each child element must occur only once

<xs:element nmae="person">
<xs:complexType>
<xs:all>
<xs:element name="firstname"type="xs:string"/>
<xs:element name="lastname"type="xs:string"/>
</xs:all>
</xs:complexType>
</xs:element>
note: once we use all indicator you can set the minOccurs  indicator to 0 or 1
maxOccurs indicator can only set to 1

Choice indicator
========================
specified one child element or another can occur
<xs:element namae="servlet">
<xs:complexType>
<xs:choice>
<xs:element name="servlet-class"type="xs:string"/>
<xs:element name="jsp-file" type="xs:string"/>
</xs:choice>
</xs:complexType>
</xs:element>

sequence indicator
==============
specifies the child element must appear in a specific order.
<xs:element nmae="servlet">
<xs:complexType>
<xs:sequence>
<xs:element name="servlet-name"type="xs:string"/>
<xs:element name="servlet-class" type="xs:string"/>
</xs:sequence>
</xs:complexType>
</xs:element>

Occurence Indicators
===================
maxOccurs indicator
<xs:element nmae="person">
<xs:complexType>
<xs:sequnce>
<xs:element name="firstname"type="xs:string"/>
<xs:element name="child_name"type="xs:string" maxOccurs="10"/>
</xs:sequence>
</xs:complexType>
</xs:element>

minCoours indicator

<xs:element nmae="person">
<xs:complexType>
<xs:sequnce>
<xs:element name="firstname"type="xs:string"/>
<xs:element name="child_name"type="xs:string" maxOccurs="10" minOccurs=1/>
</xs:sequence>
</xs:complexType>
</xs:element>
note: to allow an element to apear an unlimited number of times use the maxOccurs="unbounded" statement


any element
=============
<any>element enables us to extend the xml document with elements not specfied by the schema
<xs:element nmae="person">
<xs:complexType>
<xs:sequnce>
<xs:element name="firstname"type="xs:string"/>
<xs:element name="lastname"type="xs:string" />
<xs:any minOccurs=0/>
</xs:sequence>
</xs:complexType>
</xs:element>


====================================================================================================================================================

<any>
=========
element enables us to extend the xml document with elements with elements not specified by the schema.
family.xsd
==========
<xs:schema>
<xs:element name="person">
<xs:complexType>
<xs:sequence>
<xs:element name="firstname"type="xs:string"/>
<xs:element name="lastname"type="xs:string"/>
<xs:any minOccurs="0"/>
</xs:sequence>
</xs:complexType>
</xs:element>

now we want to extend the person element whith a children element In this case we can do , even if the
children.xsd
============

<xs:schema>
<xs:element name="children">
<xs:complexType>
<xs:sequence>
<xs:element name="childname"type="xs:string" maxOccurs="unbounded"/>
</xs:sequence>
</xs:complexType>
</xs:element>

Indicators
=============
<xs:all>   Child elements can appear in any order
<xs:sequence> child elements must appea in particular order
<xs:choice> only one child element can occur

minOccurs attribue  mimum number of times an element occurs the default value is 1

maxOccurs attribute   Maximum number of times an element occurs 
the default value is 1

=========================================================================
WebServices
============
Requirement
============
We need to integrate some set of Objects Which are running and developed in Different platForm to build into our System.


WebSevices is a Distibuted Technology Acieves Interoperability(Portablity across different Technologies such as Java,.Net,PHP,C,C++......)

The Other Distributed Technologies like Corba,RMi,Ejb,Dcom,C++ ....Uses Binary Format,hence the objects are Serialized into Stream of Bytes.

WebServices uses Xml Format Instead of Binary Format,Hence the webservices the data is exchanged as xml message,which is validated against xml schema(xsd) but not DTD,Since xsd additionally supports data types.In Webservices The objects are Serialized into xml message.

The WebServices Technologies such as SoAp,WSDL,UDDI are represented in xml against corresponding SChemas.

xmlNamspaces
==============
xml namespaces provide a method avoid elementname conflicts
name confilicts
==============
in xml element names are defined by the developer. when u trying to mix xml documents from different xml applications

this xml carries html table inforamtion
<table>
<tr>
<td>Apples</td>
<td>banaans</td>
</tr>
</table>

xml carries information about a table( apeice of furntiure)
<table>
<name>circle</name>
<width>10</width>
<length>125</length>
</table>

xml parser will not how to handle these differences.
Solving the name Conflict useing a prefix
===================

name conflicts in xml can easily be avoided useing a name prefix.
this xml carries html table inforamtion
<h:table>
<h:tr>
<h:td>Apples</td>
<h:td>banaans</td>
<h:/tr>
</h:table>

xml carries information about a table
<i:table>
<i:name>circle</name>
<i:width>10</width>
<i:length>125</length>
</i:table>

xml namespaces------>The xmlns Attribute

when useing prefixes in xml,a so-called namespace for the prefix must be defined
the namespace is defined by the xmlns attribute in the start tag of an element
syntax :   xmlns:prefix ="Uri"
<h:table xmlns:h="www.banany.com/tr"/>

this xml carries html table inforamtion
<h:table xmlns="http://www.w3org/tr/html12/">
<h:table>
<h:tr>
<h:td>Apples</td>
<h:td>banaans</td>
<h:/tr>
</h:table>
Default NameSapces
=======================
Defining a default namespace for an element saves us from useing prefixes in all the child elements.
It has  namespaceuri
this xml carries html table inforamtion
<h:table xmlns="http://www.w3org/tr/html12/">
<h:table>
<h:tr>
<h:td>Apples</td>
<h:td>banaans</td>
<h:/tr>
</h:table>

xml carries information about a table
<i:table xmlns:i="http://ibm.com/mathmatics">
<i:table>
<i:name>circle</name>
<i:width>10</width>
<i:length>125</length>
</i:table>

Develop a xsd file for the xml file?
note.xml
<note>
<to></to>
<from></from>
<heading></heading>
<body>Dont for get me this weekend</body>
</note>
note.xsd
==========
<xs:schema xmlns:xs="http://www.w3.org/2001/xmlschema"
targetNamespace="http://ibm.com" xmlns="http//www.ibm.com" >
<xs:element name="note">
<xs:complexType>
<xs:sequence>
<xs:element name="to" type="xs:stirng"/>
<xs:element name=from" type="xs:stirng"/>
<xs:element name=heading" type="xs:stirng"/>
<xs:element name=body" type="xs:stirng"/>
</xs:sequence>
</xs:complexType>
Explanation
==============


xmlns:xs      elements and datatypes come from the http://www.w3.org/2001/xmlschema

targetnamespace 
userdefined elements and datatypes in our schema belogs to our namespace such as
http://ibm.com

xmlns    indicate default namespace  http://ibm.com

elementFormDefault elementsmust be namespace qualified  elementformdefault="qualified"


How to refere a schema in an xml document?
schemaLocation="namespace location-of-xml"
<note  xmlns="http://www.ibm.com" xmlns:xsi="http://www.w3.org/2001/xmlschema-instance"
xsi:schemaLocation="www.ibm.com  note.xsd">

<to></to>
<from></from>
<heading></heading>
<body>Dont for get me this weekend</body>
</note>



Soap
==========
Soap protocol is simple Object Access Protocol
Soap is a Standard messaging protocol in WebService
Soap defines how messages can be structured in a way which is independent of any programming language or platform,and thus achieves Interoperability between application written in different programming languages and running on different operating Systesm.

The soap messge are represented in xml with Additional features

1)setOfRules(Encoding) for sending Messages.
2)Network protocol such as Http
3)To represent  protocol and application ..faults
4)Standard format for RPC-Style messageing
5)Extesibilitymodel

Soap NameSapce
===============
The sope message format is defined by an xml schema
The namesapace for soap1.1 version is http://schemas.xmlsoap.org/soap/envelop/"
the namespace for soap 1.2 version is http://www.w3.org/2003/05/soap-envelop"

If a sope application receives a mesage with diffent namesapce, it must generate fault(error) 
all soap elements must be namespace-qualified bcz the xml schema for soap1.1/soap1.2 specfies the 
elementFormDefault attribute is qualified.
Soap Structure
===============
The root  element of the soap messge is <soap:envelop>element
it contains optional <soap:Header> element and a single manadatory <soap:Body> element.

sample soap message format
===========================
  <soap:Envelop xmlns:soap="http://schemas.xmlsoap.org/soap/envelop/">
  <!-- Hedare element is optional -->
  <soap:Header>
  <!-- Header blocks for Security Credentials ,Transactions Ids.... xml format-->
  </soap-Header>
<!-- Body element is Mandatory -->
  <soap:Body>
Application data in xml format....
  </soap:Body>
<soap:envelop>

  <soap:Header>
  ==================
  The soap header contains xml elements that describe security Credentials,DigitalSignature,TransactionIds,RoutingInstructions,Debugging information,paymenttokents...



Soap Body
===========
All Soap messages must contains exactly one <soap:Body>element
<soap:Body> element contains the actual Application data in xml format.
The <soap:Body>element contains Either Application specific data or fault message,but not both.

<Soap:Body>element contains.
1)Xml Document Fragment
2)Procdure Call with parameters
3)Fault Message(Applicable only in case of Error response)
In Soap Request Message
=======================
The <soap:Body> element contains Application specific data(either xml Document fragment or procedure call with parameters)
In Soap Response Message
=======================
The <soap:Body> element contains Application specific data(either xml Document fragment or procedure call with parameters) or Fault messages, but not both.


Except in case of fault messages Soap does not specfiy the contents of the Body Element As long as the Body element may contains well-formed xml,The application specific data can be anything.

The format of the soap body is determined by MessageStyle. The soap Supports 2 Messageing Styles

1)Document----->xml document
2)Rpc---------->procedure with parmaters

The xml Data is soap body must be validated useing set of rules These rules are determined by Encoding Style.
The soap supports 2 Encoding Styles.
1)Soap Encoding
It means xml data is validated against soap encoding rules defined in section 5 of soap 1.1 specification.The soap encoding is not supported by WS-I Conformant, bcz it iteroperability problems. The soap enncoding is deprecating soap 1.2 versions. 
note:Soap Encoding is not recommeded to use.
2)Literal Encoding
It means that the xml data is validated against its xml schema.

Based on Messageing Style and Encoding Style there are 4 messageing modes supported by soap

1)Document/Literal--->xmlscema
2)Rpc/Literal--->interface methods,parameters
3)Rpc/Encoded
4)Document/Encoded

The Basic profile permits the use of Document/Literal or Rpc/Literal 

The Rpc/Encoded and Document/Encoded modes are explicitly prohibited.

1)Document/Literal
=====================
In the Document/Literal mode of messageing a soap body contains xmlDoumentFragment validated against our xml schema namespace.
purchaseorder.xsd
==================
<xs:element name="purchaseOrder">
<xs:complexType>
<xs:sequence>
<xs:element name="AccountName type="xs"string"/>
<xs:element name="AccountNumber type="xs"string"/>
<xs:sequence>
xml
===
<purchaseorder>
<accountname></accountname>
<accountnumber></accountnumber>
</purchaseorder>
<soap:body>

The xml element name from our schema becomes direct sub elements of the <soap:body>
<soap:Envelop xmlns:soap="http://schemas.xmlsoap.org/soap/envelop/">
<soap:Header> <!-- heder block here-->
</soap:Header>
<soap:Body>
<!--Xml Document Framgement-->

<tns:purchaseOrder xmlns:tns="www.crescentits.com/po"
<AccountName>shvia.com</AccountName>
<AccountNumber>123</AccountNumber>
</tns:purchaseOrder>
</soap:body>
</soap:Envelop>

RPC/Literal
===================
The RPC/Literal mode of messaging specifies how methods and their parmeters and return values are represented within the<soap:Body>element.
The Rpc request message contains the method name and the input parameters
An Rpc response message contains the return value and any output parameters (or a fault)

ServiceEndpointinterface(SEI)

pulbic interface Book extends java.rmi.Remote
{
public float getBookPrice(String isbn)throws RemoteException,InvalidException;
}

RPC/Literal soap Request message
===========================

<soap:body>
<!-- method name becomes subelements of the soap body element-->
<tx:getBookPrice>
<!-- parameternames becomes child Elements-->
<isbn>12544</isbn>
</tns:getBookPrice>
</soap:body>

RPC/Literal soap Response message
===========================

<soap:body>
<tns:getBookpriceResponse>
<result>1254</result>
</tns:getBookpriceResponse>
</soap:body>
Rpc-Style messageing is a common in distributed technologies,including corba,dcom,and others,so soap defines a standard xml format for rpc-style messageing.called rpc/literal.
Conclusion: when we say a mesaging mode is Document/Literal or Rpc/Literal, we are usually Describing the payload of the sope message. An xml document frgment or an xml representation of the parameters and return values associated with a remote procedure call.

Soap Faults
================
the <soap:fault> element is added to <soap:body> in soap reponse message in case of an Error.
<soap:fault> element contains child elements
<soap:Code>
<soap:Reason>
<soap:nodeminOccurs=""/>
<soap:RoleminOccurs="0"/>
<soap:DetailsminOccur="0"/>
<soap:Code> defines a small set of soap codes covering hight level soap faults.

versionmismatch   soap 1.1 and soap1.2 version mismatch between soap send and soap Receiver ,Wrong Envelopnamespace.
mustUnderstand
==============
DataEncodingUnknown


soap over http
==================
the soap message can be transported over many different network protocols useing set of rules is called as soap binding. The standard network protocol used for soap is http.
Soap message sent over http are placed int0 the payload of an http request or reponse 
http is a Request/Response protocol,which means that the sender expects respnse (error or data) from the Receiver.

WebServices that use soap over http is always use http post but not http get since post request hv a payload area and is perfectly suited to carrying soap message.


ex: Soap requst over http

post
host
content_type
soapAction=""

WSDL
========
Wsdl document is used to provide descripton about webservice such as interface name,methodnames,parameter types,Returntypes, in xml format.
It provides message format(such as soap),Networkprotocol(such as http),and EndpointAddress(UrI)that client must use to communicate with a Service
Note:
wsdl document-->
 is used to provide description about web service such as
 interface name,methodnames,parameterTypes,return type in xml format.
it provides message format(such as soap),network protocol(such as Http)
and endpoint address(uri)

Basic Structure of WSDL
========================
Wsdl is schema based document whose name is http:schemas.xmlsoap.wsdl/
the wsdl document contains 7 important elements:
Definations,types,message,porttype,operations,binding and service
<wsdl:definitation>is the root element of the wsdl document.
<wsdl:types>elements used xml schema language to declare applciation specific xml data types,xml elements,and Exception types.


<wsdl:message>element descirbes the payload of a message useing xml schema simpleTypes,ComplexTypes,or application specific xml types(or xml elements)defined useing <wsdl:types>
<wsdl:portType>element defines ServiceEndpointInterface(SEI)This is analogous to a java interface.
<wsdl:operaton>element describes one method in sei.The element uses input,output,fault messagetypes.

<wsdl:binding>element is used to specify message format (such as soap format),http,smtp..message style (such as rpc or document) encoding styles(literal or soap encoding)

<wsdl:service> element responsible for assigning an EndPoint address(uri) to a specific port(binding)

<wsdl:definitions targetNamespace="http://www.cresentits.com">

xmlns:soap="soapnamespace"
xmlns:wsdl="wsdlnamespace"

<!-- Define application specifc xml element names and element types including application specific excetion types,element names are required in case of Document Style messaging-->
<wsdl:types>
<xsd:schema>
</xsd:schema>
</wsdl:types>

<!-- message elements describe the input ,output,fault message--->
<!-- input message-->
<wsdl:message>
<!-- can hv multiple parts-->
<wsdl:part/>
</wsdl:message>
<!-- out put message-->
<wsdl:message>
<!-- can hv multiple parts-->
<wsdl:part/>
</wsdl:message>
<!-- fault message-->
<wsdl:message>
<!-- must hv only one part-->
<wsdl:part/>
</wsdl:message>

<!-- PortType element describes the absract interface webservice.It becomes a serviceEndpointe Interface in java-->
<wsdl:portType>
<wsdl:operation>
<!-- must hv single input element-->
<wsdl:input/>
<!-- atmost one output element-->
<<wsdl:output/>
<!-- zero or more fault element-->
<wsdl:fault>
</wsdl:operation>
</wsdl:portType>



<!--element is used to specify message format (such as soap format),http,smtp..message style (such as rpc or document) encoding styles(literal or soap encoding)-->
<wsdl:binding>
<soap:binding style="rpc/document"/>
<wsdl:operation name="--">
<soap:operation soapAction="--"/>
<wsdl:input>
<soap:body parts="" use="literal" encodingStyle="" namespace=""/>
<wsdl:output>
<soap:body parts="" use="literal" encodingStyle="" namespace=""/>
<wsdl:fault name=--"
<soap:fault name="--"use="literal" namespace="--"/>

<!-- conains set of ports ,each referes specific port .This element maps with sei in java-->
<wsdl:service>
<wsdl:port>
<soap:address locaation="endpoint uri"/>
</wsdl:port>
</wsdl:service>


note: the targetname contains all the elements and elementtypes defined in the schema. it contains port types,operations,bindings,ports......


<wsdl:Types>
================
element uses xml schema language to declare applications specific xml data types,xml elements,and exception types.

In case of DocumentStyle messageing the element names must be defined
eg:
note: targetnamespace contains all the element and elemnt types defined in the schema
<wsdl:types>
<xsd:schema targetNamespace="http:www.cresentits.com/ss/">
<xsd:element name="concatRequest">
<xsd:complexType>
<xsd:sequence>
<xsd:element name="s1" type="xsd:string"/>
<xsd:element name="s2" type="xsd:string"/>
</xsd:sequence>
</xsd:complextype>
</xsd:element>
<xsd:element name="concatResponse" type="xsd:String">
</xsd:schema>
</wsdl:types>
in xml
<concatRequest>
<s1></s1>
<s2>/s2>
</concatRequest>
in case of Rpc style messageing element names not reuqired but optionally element types,exception types can be declared...

<wsdl:types>
<xsd:schema targetNamespace="http:www.cresentits.com/ss/">
<xsd:simpleType name="firstname"
<xsd:restrictio base="xsd:string">
<xsd:pattern value="[a-z][A-Z]"/>
</xsd:restriction>
</xsd:schema>
<xsd:complexType name="InvalidSymbolException">
<xsd:sequence>
<xsd:element name="message" type="xsd:stirng"/>
</xsd:sequence>
</complexType>
</wsd:types>


<wsdl:message>

The message element for Document style webservices
<wsdl:types>element doument style messaging exchanges xml document and refere to the top level elementname.
In document style messaging we can use only one part element the name attribute of the<part>element is unimportant but required for wsdl validation.
we hv to use 'element' attribute of <part>element
eg:
====
<wsdl:definiations>
<wsdl:types>
<xsd:schema targetNamespace="http:www.cresentits.com/ss/">
<xsd:element name="concatRequest">
<xsd:complexType>
<xsd:sequence>
<xsd:element name="s1" type="xsd:string"/>
<xsd:element name="s2" type="xsd:string"/>
</xsd:sequence>
</xsd:complextype>
</xsd:element>
<xsd:element name="concatResponse" type="xsd"String">
</xsd:schema>

</wsdl:types>

<!-- message elemens desc ribe the input and out put messages-->
<wsdl:message name="ConcatRequest">
<wsdl:part element="concatRequest" name="parameters"/>
<wsdl:message>
<wsd:message name="concatResponse">
<wsdl:part element="concatResponse" name="parameters"/>
</wsdl:message>
</wsdl:definiation>

The message Element for Rpc -Style webServices
================================================
IN case of Rpc -style messageing the message element describe the payloads of the soap request and soap response messages such as parameter types,returntypes ....

Can hv multiple partelements The name attribute is required which becomes mehtod parameter name. the type attribute referex xml  datatype,may be built-in or application specific data.

ex:
----
<!--input message-->
<wsdl:message name="concatRequest">
<!-- can hv multiple part element the name attribute is required which becomes method parmeter name the type attribute referes xml data type-->
<wsdl:part name="s1" type="xsd:string"/>
<wsdl:part name="s2" type="xsd:string"/>
</wsdl:message>
String concatRquest(String s1,String s2)
<!--output message-->
<wsdl:message name="concatResponse">
<!-- can hv multiple part elements-->
<wsdl:part name="return" type="xsd:String"/>
</wsdl:message>
//In case of Rpc-Style messaging th epart element must use the type attribute which indicates parameter type or return value.
<!-- fault message-->
<wsd:message name="Exception">
<!-- fault message always contains single part,which becomes exception message in java-->
<wsdl:part name="InvalidSymbolException" type="xsd:string"/>
</wsdl:message>


<wsdl:portType>
==================
A portType defines the abstract interface of a webservice It is analogous to java Interface.
PortType element contains operations without implementation detials. such as interface is called as ServiceEndPointInterface(SEI)
In wsdl the port type is implemented by the binding and service elements, which provides information about messageformat,transportprotocol,mesageing style,encoding style,uri for service .

eg:
<wsdl:portType name="simpleService">
</wsdl:operation>
</wsdl:portyType>

public interface simpleService implements java.rmi.Remote
{

//operations
}

<wsdl:operation>
====================
Each operation is composed of one input,one output element and any number of fault elements.

In case of DocumentStyle Messageing
===================================
name attribute of<operation>element is not used in soap message but required for wsdl file validation.the name attribute is required for wsdl2java tool to generate skeleton and stub classes.
eg:
<wsdl:portType name="simpleService">
<wsdl:operation name="concat">
<wsdl:input message="tns:concatRequest"/>
<wsdl:output message="tns:concatResponse"/>
<wsdl:operation/>
</wsdl:porttype>

//java Interface
public interface simpleService
{
public concatResponse concat( ConcatRequest  concatRequest);
}

In case of Rpc Style messaging the name attribute of<operation>element becomes method name in web.

<wsdl:portType name="simpleService">
<!-- name attribute is mandatory which is method name in service-->
<wsdl:operation name="concat">
<wsdl:input message="tns:concatRequest"/>
<wsdl:output message="tns:concatResponse"/>
<wsdl:fault name="InvalidSymbolException" message="tns:invalidsymbolexception"/>
<wsdl:operation/>
</wsdl:porttype>

//java Interface
public interface simpleService
{
public String concat( String  s1,String s2);throws invalidSymbolexception
}

class InvalidSymbolException extends Exception
{
-------
}

An input message represent the payload send to the webservice ,and the output message represents the payload send back to the client.
In rpc input is a request,output is a response.

in DocumentStyle messageing the input is the xml document sent to the webservice,and the output is the xml document fragment back to the client.

In,Out,Inout parameters
==========================
in parmater are native to java.out and inout parameters are not.
To accomadiate out and inout parameters jax-rpc defines the javax.xml.holders.Holder interface.

ex:
void main(Stirng[]arg)
{
int a=1;
String name=new String("shiva");
meth(a,name);
s.o.p(a);//1
s.o.p(name);//java
}
void meth(int a,String name)
{
a=2;
name=new String("java");
}
note: pass-by-copy parameter are known as in parmaters All modern progrmming language support in parmaters.

pass-by-Referece: Inout and out parameters
===============================================
java does not support pass-by-Referece .jax-Rpc uses Holder classes to support pass-by-Referece.
Other programming languages.c++,C#,perl.......

eg:
void main()
{
int a;
system.DateTime today=System.DateTime.Now;
foo(a,today);
s.op(a);//5
sop(today);//change date will be reflect.
}

public void foo(in parma1,ref system.DateTime param2(
param1=5;
param2=new Date(1980,1,1);
}


eg1:
void main()
{
int a;
system.DateTime today=System.DateTime.Now;
foo(a,today);
s.op(a);//5
sop(today);//change date will be reflect.
}

public void foo( outint parma1,out system.DateTime param2(
param1=5;
param2=new Date(1980,1,1);
}


Holder: Supporting Inout and Out parameters useing jax-RpC
====================================================
eg: A c# WebService that uses input and out parameter
public class fooBar
{
public void foo(ref int param1,out system.DateTime param2)
{
param1=param1+5;
param2=new System.DateTime(1952,1,1);
}

Eg: A jax-Rpc endpointInterface that supports inout,and out parameters useing Holder classes.

public interface FooBar extends Remote
{
public void foo(intHolder param1,CalendarHolder param2)throws RemoteException
}

eg:
======
Client code
intHolder i=new IntHolder(10);
CalenderHolder h=new CalenderHolder();

note the value of a Holder clas is always available via the public static variable named value.

Mapping Holder Types From Wsdl
================================
Jax-Rpc creates stubs from wsdl document. It is important to understand how input,and out parameters are defined in wsdl and mapped to jax-rpc endpoints.

eg:
====
<message name="fooRequest">
<part name="param1"type="xsd:int"/>
<part name="param2" type="xsd:double"/>
</message>
<message name="fooResponse">
<part name="param2"type="xsd:int"/>
<part name="param3" type="xsd:dateTime"/>
<part name="param4" type="xsd:xsd:float"/>
</message>
<portyType name="FooBar">
<operation name="foo" parameterOrder="param1param2param3">
<input message="tns:fooRequest"/>
<output message="tns:fooResponse"/>
</operation>

<operation name="foo1" parameterOrder="param1param2param3param4">
<input message="tns:fooRequest"/>
<output message="tns:fooResponse"/>
</operation>
</portType>

Base on this EndPointInterface Generated .
public interface FooBar extends Remote
{
public float foo(int param1,DoubleHolder param2,CalenderHolder param3)throws RemoteException
public void foo1(int param1,DoubleHolder param2,CalenderHolder param3,FloatHolder param4)throws RemoteException
}

note: In wsdl the operation names cannot be same since they cause interoperability problems, hence the BasicProfile prohibits operation oberloading.

Rules
==========
1)If a part name is delcared only by input message,then its an in parameter,which doest not require Holder type.
2)if same part element both input and output message, thenit is INOUt parameter.Hence Holder class is required.
3)If the part element is only defined in the output message,indicating that it is either Return value or an out parameter .if the par name is listed in parameterOrder attribute, then it is out parameter.Other wise it is Return value.Holder class is required for Out parameters,but not required for return type.
note: Return type and out parameter are almost same but not exaclty same.
4)if the parameterOrder attribute is declared then all input message parts must be listed the output parts may or may not ble listed.
5)if there is a single unlisted output paramter,then that parameter is the return type of the method. other wise return type is void.
a)if all out part elemnet listed i parameterorder attribute then return type of the method is void.
b)if more than one part elements are unlisted in parmeterorder attribute.then return type of the method is void.


Messaging Exchange Pattern
=================================
there are 4 basic message exchange patterns.
1)Request/Response
2)one-way
3)notification
4)Solicit/Response

The Basic profile supports only Request/Response and ONe-way messageing.

Request/Response messaging
===========================
The client sends a Reuqest message and the webservice replies Response message.Hence It is Synchronous messaging.
The< wsdl:operation>inludes one <wsdl:input>one <wsdl:output>element and zero or more <wsdl:fault>elements

eg:
====
<wsdl:portType name="BookQuote">
<wsdl:operation name="getBookPrice">
<wsdl:input message="tns:getBookPriceRequest">
<wsdl:input message="tns:getBookPriceResponse">
<wsdl:fault name="InvalidArgumentFault" message="tns:InvalidArgumentFault">
<wsd:fault name="securityFault" message="tns:securityFault"/>
</wsdl:operation>
</wsdl:portType>
One-Way messaging
===============
The client send a Request message to a webservice but doesnt expect reply message Hence it is Asynchroousmessaing.
<wsdl:operation>includes only<wsdl:input>element without <wsdl:output>and <wsdl:falut>elements.
eg:
<wsdl:portType name="BookQuote">
<wsdl:operation name="getBookPrice">
<wsdl:input message="tns:getBookPriceRequest">
</wsdl:operation>
</wsdl:portType>

<wsdl:Binding>
==============
<wsdl:binding> element is used to specify for every <wsdl:portType>
1)Message format(such as soap format,http format)
2)transport protocol(http,smtp)
3)messaging style(such as Document or Rpc)
4)encoding Style (such as literal or soap encoding.)

eg:
====
<wsdl:binding name="SimpleServiceSoap" type="tns:SimpleService">
<soap:binding transport="http://schemas.xmlsoap.org/soap/http" sytle="....">
-
<wsdl:operation name=".......">
<soap:operation soapAction="........" style="....."/>
-
<wsdl:input>
<soap:body use="......" namespace="......"/>
</wsdl:input>
-
<wsdl:output>
<soap:body use="......" namespace="......"/>
</wsdl:output>
<!-- <wsdl:fault> and <soap:fault> elements includes a mandatory name attribute which Referes to a specific fault message-->
<wsdl:fualt name="---"/>
<soap:fault use="......" name="......"/>

</wsdl:operation>
</wsdl:binding>

type type attribute referes portType.
the children of the <wsdl:binding>element (operation,input,output,fault)
map directly to the corresponsing children of the portType element.

<soap:binding>
================
The <sope:binding> element specifies message format (in the case soap format).
TransportProtocol,used to transport soap message and teh default message style  its operations.
eg:
<soap:binding transport="http://schemas.xmlsoap.org/soap/http" style=document"/>

<wsdl:operation>
the name attribute of <wsdl:operation> referes method name .this is mandatory attribute.

In case of rpc style messaging the value of the name attribute is the methodname and which is used to gnerated soap message.


<soap:body>
element is used to specify Encoding style
element hv 4 attributes use,encodingsylte,namespace,parts


===================================================================================================
WebServices Implementation
============================
Q)What is WS-I?
The ws-i(WebServicesInteroperability)organization is an association of It industry
companies,including ibm and microsoft,that aim to create webservcies specficiation
that all companies can use.
Q)What are the differnt standards given by WS-I to implement webservices?
Ws-i given 
BasicProfile1.0(Bp 1.0)
BasicProfile1.1(Bp 1.1)
BasicProfile2.0(Bp 2.0)
q)what are webservices?
There are so many api, iplementation for the ws-i given standards
sun has released "Jax-Rpc" api that follows Bp1.0 standard
sun has released "Jax-ws" api that follows Bp1.1 standard

specification     Api                      Implementation
(From Ws-I)       (From sunmicro)          (from different companies)

Bp1.0               Jax-Rpc                  Jax-Rpc-Si(fromsun),Apache-Axis(fromasf)...

Bp1.1                jax-ws                 Jax-wsRi(fromSun),apache-axis2(fromasf),metro(From sun),cxf(from asf)...

note:Jax-ws Ri(Reference implementatio)was failed to access by .net,means failed interoperability,sun then relaesed "metro" implementation of jax-ws,which resolved interoperability problem and also added some more features.

Note: Apache CXF Internally uses spring.





WEB SERVICES DEVELOPMENT 

WEBSERVICES DEVELOPMENT CAN DONE IN TWO WAYS

1)CONTRACT FIRST(TOP-DOWN)
WSDl---->Services
2)CONTRACT LAST(BOTOM-UP)
services--->wsdl

note:services can be developed with any technology like .net,java,php......
In java,servcies can be developed using any api like jax-rpc,jax-ws,jax-rs.....
In  java servcies can be developed using any implementations like sun,apache......
But WSDl development is unique its not plat form specific,not language specific,not technology specific, not api specific,
not implementation specific

So, We can say we are developing Webservices using
JAX-RPC ,CONTRACT FIRST APPROACH
JAX-WS,CONTRACT LAST APPROACH
NOTE: So, we can say we are developed webservcies useing jax-rpc,jax-ws,jax-rs

note: In the internet world we prefer to use Http protocol, and we hv so many technologies which supports
http protocol,

q)What are the  http protocols implemented apis?
ServletApi
Ejb Api

q)What is EndPoint/SEI/SEA?

A component which receives Consumer request 
In General we use either servlet or ejb as an EndPoint.

so we can say we are developing web servcies using 
jax-rpc,servlet end point url,contract frist approach
jax-rpc ,ejbendpoint url contract last approach

MEP
======
 Message Exchanging patterns
 Consumer can communicate with provider in three ways
 Synchronous request-reply
ASynchronous request-reply
fire and forget

 Synchronous request-reply
=============================
In this consumer sends a request to provider and consumer blocks until response comes back from the provider
until response comes back consumer cant proceed.
ASynchronous request-reply
============================
in this consumer sends the request to provider and consumer will not wait until it gets the response.
After request sent to provider it continues it flow of execution.
Consumer will hv one response Listener which listens the response from the provider.

Fire and Forget
==================
In this consumer send the request to provider and consumer will not wait until it get the response even it wont hv any response listener
Once the request is sent to the provider it contineus its process,doesnt bother about response.

So,we can say we are developing webservices useing 
Jax-Rpc,Servlet endpoint url,Contractfirstapproach,Synchronousrequest-reply
Jax-Rpc,Servlet endpoint url,Contractfirstapproach,ASynchronousrequest-reply
Jax-Rpc,Servlet endpoint url,Contractfirstapproach,fire and forget

Mef
====
Message Exchanging Formats
When consumer,provider exchanging the information,that information can happen in the formats,
Document-literal
rpc-literal
rpc-encoded
document-encoded

Literal--->As its is xml is Exchaging 
ecoded--->utf-8,utf-16

Default Mef is rpc-encoded
So,we can say we are developing webservices useing 
Jax-Rpc,Servlet endpoint url,Contractfirstapproach,Synchronousrequest-reply,rpc-ecoded
Jax-Rpc,Servlet endpoint url,Contractfirstapproach,ASynchronousrequest-reply,rpc-literal
Jax-Rpc,Servlet endpoint url,Contractfirstapproach,fire and forget ,document-literal

q)How the provider and consumer communicate in Distribute Technology?

======================================================================

So, we dont send raw xml document(contains buseinss data)to the providers
 To aheive this we will go to soap
 Soap stands for simple objectaccess protocol
 soap is a classfication protocol
 soap is a binding protocol(processing data+businesdata)


 But what services are providing by the provider should be explained.To know
 the services of provider,Consumer cannot look intothe code of provider
 So consumer need the information like what are the services are providing,
 what they will take as input,and what the ouput they will return.

Provider will explain all these in one document called  Wsdl

wsdl stands again is an xml document ,bcz it should be language independent,
so that any type of client can understand the services of the provider

wsdl is the document which explains the services information.But how can 
Consumer  get the wsdl document,from where Consumer Get?

sO,Wsdl documents has to be placed in some location from where Consumer can access them,that location is nothing but UDDI

UDDI Stands for Universal Description Discovery and Integration.
Uddi is the Registry where all the wsdl documents are registred.
UDDI also should be interoperable,so it again developed in xml 
UDDI registry also called XMLRegistry.


AXis
=================
Soap specification can be implemented using any programming lanague such as java,.net,..
It is up to the service provider to choose programming lnaguage for writing webservice and appropriate soap Runtime Environment
To use java as programming language to develop soap based webservices,the corresponding soap runtime enviroment should be implemeneted in java

A long list of open source communites (such as Apache Axis2),Webservices platform providers (such and java,.net),j2eevendors(weblogic,websphere)hv release theri soap runtime enviroments.
Out of many vendors who provided soap runtime environment in java , but popular among all is Axis2.
Aapache Axis2 is an open source soap implementation that provides environement for writingsoap based webservicepplication.
