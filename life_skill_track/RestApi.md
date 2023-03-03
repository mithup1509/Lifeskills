# REST

## HISTORY
 in **2000** a Web **API**s was Recognized.a group of experts ,led by **Roy Fielding**, Invested **REST**,and phd thesis presents Architecture Styles & Design of Network base Software Service.
 They Started purpose was Simply to Create a Standard that allows two server to communicate and exchange data anywhere in the World.**REST** is a software architecture style that describes the architecture of the Web. REST We have data in Server is called State,if client need that data means client send the request to the server and server send the data to the user and server doesn't send password like important data.it send the data in the format of **JSON**,**XML**.

![RestApi](https://www.mindinventory.com/blog/wp-content/uploads/2022/10/rest-api-model-1.png)


1. [what is API](https://g.co/kgs/3gmHEP)  
1. [what is Rest](https://g.co/kgs/tixZRC)
1. [types of Web Api](https://www.techtarget.com/searchapparchitecture/tip/What-are-the-types-of-APIs-and-their-differences)



## What is REST Architecture

* **REST** Stands for **RE**presentational **S**tate **T**ransfer.
* **REST** is Web Standards based Architecture and uses **HTTP** Protocol.
* Here every Component is a Resource.
* Resources are accessed by common interface using **HTTP**.

## What is Resource

*  in **REST** architecture every content is a resource.
* These resources can be a 
    * text files
    * HTML pages
    * Images
    * Videos.
* **R**esource can be identified by **URI**s.
* **REST** is a client access and modifies the resources.
* **REST** is Server Simply provide access to Resource.
* **REST** uses various Representations to represent a resource 
    * **JSON**
    * **XML**

## Constraints
* client-server
    * Server host the resources ,client request the operation on resource.
* Statelessness
    * no Assumption State to implements Apis and idempotent.
* Cacheability
    * coaching based on Server Responce.
* Layered System
    * No assumption on client identity.
    * loose coupling to client & promies.
* Code on Demand
    *Dynamic Responce.
* Uniform interface
    * Representation of resource state with uniform data model.

## Why REST HTTP based API
* **HTTP** already executed in 2000
* **HTTP** implements Client/Server architecture
* **HTTP** method state transfer request of REST 

## Resource Representation in json

```json
an Employee data in JSON can be a resource
{
    "ID":7,
    "NAME":"MITHUNKUMAR",
    "AGE":23,
    "ROLE":"SOFTWARE ENINEER"
}

```

```json
Country Temprature 
{
    "country":{
        "city":{
            "temp":23,
            "humidity":45
        }
    }
}

```

## Resource Representation in XML
```xml
<country>
<city>
<temp>23</temp>
<humidity>45</humidity>
</city>
</country>

```

in **HTTP** there are five methods that are commonly used in a **REST**-based Architecture i.e.,**POST**,**GET**,**PUT**,**DELETE**.these coorespondent to CREATE,READ,UPDATE and DELETE (or **CRUD**)   operations respectively. there are other methods which are less frequently used like OPTIONS and HEAD.
* **GET** : the HTTP GET method is used to **read**(or retrieve) a representation of a resource.In the safe path,GET returns a representation in XML or JSON and an HTTP response code of 200(OK).

* **POST**: the POST verb is most often utilized to **create** new resource.on successful creation ,return HTTP status 201,returning  a location harder with a link to the newly created resource with the 201 HTTP status.
   
    **POST** is neither safe nor idempotent.
* **PUT**: It is used for updating the capabilities.**PUT** can also be used to crate a resource in the case where the resource **ID** is choosen by the client instead of by the server.on  successful update,return 200(or 204 if not returning any content in the body)from a **PUT**.

* **DELETE**:it is used to delete a resourse identified by a **URI**.on Successful deletion ,return HTTP status 200(OK) along with a respone body.

```java
a=5 //it is idempotence,as final value (a=5)
    //would not change after executing it multiple times 
a++ //it is not idempotence because the final value will 
    //depend upon   the numberof the timesthe statement will executed

```

![rest](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_LEvQzaWnXSWs7Z-BLcpYIAyLViGQxtq51oa13DapeWPalp7evhpn4gbOD6EVwvJGRRQ&usqp=CAU)



## Request and Response
We will see how request and responce work for **HTTP** methods.
* **GET**: Request for all students.
      Request
  GET :/api/students
* **POST**:Request for posting/Creating/Inserting Data
      Request
  POST:/api/students
  {"name":"RAJ"}
* **PUT** :Request for updating Data at id=1
    Request
  PUT :/api/students/1
  {"name":"RAJ"}     
* **DELETE** Request for Deletig Data of id =1
    requst
   DELETE:/api/students/1


**API** stands for Application  Programming Interface Which is a Software Intermediary that allows two application to talk to each other.An api is a software which can be used to communicate with other software or even hardwares.

## What is an Endpoint
An endpoint is a simple URL through which you can use an API (or a Web API)

## Resourse URI
  **U**nique **R**esource **I**dentifier
  it identify the state resource uniquely in server store.

  **NOUN BASED ONLY**

  ex:

  /product

  /item

  /employee

  /student

 **NOT BASED ON VERB**

  ex:
  
  /getproduct

  /getitem

  ## Why REST is Popular

  * it based HTTP
  * backward compatibility
  * Reasanability easy
  * Scalability 
  * Idempotent
  * Resonable Security

## REFERENCE
[youtube ](https://youtu.be/Xh4EvFEFZXc "explain in tamil")

[youtube](https://youtu.be/qVTAB8Z2VmA "english")

