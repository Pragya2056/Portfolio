## Introduction to REST API
![REST API](https://miro.medium.com/max/785/1*6rG4TYLov2gIoKuEcCXnNw.jpeg)


### Introduction 

REST API or REpresentational State Transfer Application Programming Interface is an architectural style that defines the rules over which the web services are to be created. It is a simple and flexible way to communicate (fetch or give information) between web services. We can also see the REST API being regarded as the “language of the internet” these days.
The REST API was first introduced by Roy Fielding and his colleagues in 2000. They wanted to create some uniform and predefined set of rules that would allow the requesting systems to access and access as well as manipulate the web resources for their benefit. 
The REST API is an alternative to a more sophisticated SOAP (Simple Object Access Protocol) technology. We can say that it is more helpful in the cases where the SOAP can be complicated because REST is much simpler than the SOAP. But we still have a question “WHY do we use REST API for more robust SOAP technology?” – This is because REST is very simple and flexible and uses less bandwidth which makes it a better choice for our internet usage. It also gives us very high performance because of caching. Further, you can see the proper documentation with the use of REST API alongside proper logging of error messages. 


Now, let us look at some basic features of the REST API: -
1.	It is very lightweight. 
2.	It is simple and standardized.
3.	It is highly scalable. 
4.	It is easily maintainable which means you can make changes with time, which is why this is the most commonly used API in web-based applications these days.
5.	The web services that follow REST API are called RESTful web services. 
6.	All the communication, as well as the interaction on the REST API, is done via HTTP (HyperText Transfer Protocol) request only. This means there is a client-server architecture for the API. 
Moving on, there are two components of the RESTful system.
![RESTful System](https://miro.medium.com/max/1050/1*z4QGnfXj0rIvftqxB7IKgA.jpeg)

Apart from these features, there are six architectural constraints of the REST API. They are the principles on which the REST API is based. They are listed out below:
1.	Uniform Interface				
2.	Stateless
3.	Cacheable
4.	Client-Server Architecture
5.	Layered System
6.	Code on Demand
Among these six constraints, the first five are never to be disturbed because even if we try to violate just one, it will no longer fall under the RESTful system. However, the last one, Code on Demand is an optional constraint of REST API. It will be better if it is there, but it will still be the RESTful system if it is violated in some way. Let’s see all these points one by one in brief.
1.	Uniform Interface
The first one is the Uniform Interface which is a key principle that can differentiate between a REST API and a Non-REST API. This states that despite the type of device or an application, it should have a uniform way of interacting with the given server. It is further categorized into four guidelines: -
a)	Resource-Based
This states that the individual resources here are identified in requests.
b)	Manipulation of Resources through Representation
This states that a client has the representation of resources that has about enough information to make some changes (Modify or Delete) the resource on the server if you have the permission to do so. 
c)	Self-descriptive messages
As the heading suggests itself, each message comes with enough information so that the server can easily analyze the request without looking up the process. 
d)	HATEOAS
HATEOAS or Hypermedia as the Engine of Application State tells us that we need to include links for each response on the server so that a client can realize the other resource with the least effort. 
2.	Stateless
Further, the next constraint is stateless which means all the required states to look over the request is included within the request itself. The server will not store anything that relates to any of the request sessions. 
3.	Cacheable
Next, we have cacheable which specifies that each response should include whether it is cacheable or not. It also mentions the durations for which the responses can be cached on the client-side. This results in high performance because the resources are saved in the cache memory and returned very fast. 
4.	Client-Server Architecture
As mentioned earlier, the RESTful system should have a client-server architecture. 

![Client-server architecture](https://miro.medium.com/max/1050/1*NU34CAD64ToUf0GP5ekKxQ.jpeg)

5.	Layered System
Any application architecture should always be in multiple layers. The more the layers, the more stable and secure the architecture is. Multiple layers limit the component behavior while also enabling load behaving which makes it very stable. They also provide shared caches that promote scalability. 
Moreover, the application security is very high because of the multiple layers because a layer can only communicate with its immediate layer and none of the other layers. 
6.	Code on Demand (optional)
Finally, there is Code on Demand which I mentioned earlier about being an optional constraint of the REST API. This states that the servers can provide executable code to the client for them to make changes. For Examples - Java applets and client-side scripts like JavaScript. 
After the principles of REST API, we now move on to understanding how the HTTP protocols are used in the Interface. We can send a proper HTTP code in the REST API which indicates a success or error status. 
As we know, we commonly use the CRUD operations for the protocol. Let’s see “What is CRUD?”
CRUD stands for Create, Read, Update, and Delete operations. In REST API, it corresponds as follows:
•	Create = POST
It is used to create resources. We can say it sub-ordinates resources. 
•	Read = GET 
It helps read a representation of the resource. 
•	Update = PUT
This updates the capabilities of the resources. It can also be used to create a resource where the resource TD is given by the client and not the server. 
•	Delete = DELETE
Finally, we can use the DELETE command to delete a resource identified by a URI. 
We can also see a fifth command that is used as much as these. It is called PATCH and it modifies the capabilities where we can use just a patch instead of the whole resource. In addition, the OPTIONS and HEAD commands are very less used.  
To understand these commands better, let’s study the table below which tells us a little more about them. 


![Commands](https://miro.medium.com/max/1050/1*ALfXgMSqLs32SpAsHHYATw.jpeg)

Here, you can see how we have used the commands to accomplish various CRUD operations.
NOTE: You can use the GET and POST commands with no problems but if you need to use the PUT and DELETE commands, you need to install method override. To do this, you can use the following command: - 

![install method override](https://miro.medium.com/max/1050/1*cq_aaq-ToyIrBkwZfAtz3g.jpeg)

This also requires you a package that you can acquire by the following command: -

![To get the package](https://miro.medium.com/max/1050/1*TC4Wv1mzIOLiM7n_TyOTnw.jpeg)

Now, to use it, 

![To use it](https://miro.medium.com/max/1050/1*WCGUdnIOsHo0QKxqBzLdiQ.jpeg)

## Are there any alternatives to REST API?

Although REST API is the most commonly used API on web-based applications nowadays, you can also use its alternatives. There are many of them among which, there are some we have listed out below: -
1.	GraphQL APIs
2.	Falcor APIs
3.	gRPC APIs
4.	JSON-Pure APIs
5.	oData APIs
