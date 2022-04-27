**1.** What is API? Give 3 real-life examples of usage of API. <br/>
**Answer:** API stands for Application Programming Interface. It works as an intermediary between two apps for them to communicate with each other. <br/>
        **Example - 1:** When using travel sites like Kayak or Expedia to book a flight the travel sites interacts multiple airline's API to aggregate all the data and show it to us. <br/>
        **Example - 2:** Similarly when using Google Maps, if we are looking for directions to a certain place most of the time there is an option to book a ride from different ride hailing apps. In this case Google Maps is using the rideshare app's API to request information by sending a HTTP request function. The rideshare app's API then sends the requested information. <br/>
        **Example - 3:** Many app allows us to sign in through Google, Facebook or certain other popular social media accounts. Like Postman where we can sign in through our Google credentials. Postman uses Google's API to verify the user's identity along with certain other valuable information it needs. <br/>

**2.** What is API testing and name some types of API testing?<br/>
**Answer:** API TESTING is a software testing type that validates Application Programming Interfaces (APIs). The purpose of API Testing is to check the functionality, reliability, performance, and security of the programming interfaces. Some examples of API testing would be Performance Testing, Load Testing, Runtime Error Detection, and Security Testing.<br/>

**3.** What is the difference between REST and SOAP APIs?<br/>
**Answer :** SOAP(Simple Object Access Protocol) is a protocol and thus follows a strict standard to allow communications between the client and server whereas REST(REpresentational State Transfer) doesn't follow any strict standard but follows six specific constraints. Those constraints are – Uniform Interface, Client-Server, Stateless, Cacheable, Layered System, and Code on Demand.<br/>

**4.** What are common HTTP methods? Explain with examples.<br/>
**Answer :** There are 5 commonly used HTTP methods. They are Post, Get, Put, Patch, and Delete.<br/>
            **Examples :**<br/>
            **Post :** Creating and article in a block.<br/>
            **Get :** Loading a webpage.<br/>
            **Put :** Updating all fields in an article in a blog.<br/>
            **Patch :** Updating specific fields in an article in a blog.<br/>
            **Delete :** Remove an article on a blog.<br/>

**5.** What is the difference between POST AND put? Explain with an example.<br/>
**Answer :** POST means "create new" as in "Here is the input for creating a user, create it for me". <br/>
             PUT means "insert, replace if already exists" as in "Here is the data for user 5".<br/>

**6.** Name 5 main categories of HTTP status codes? Explain 5 status codes from each category(You have to tell the status code and description of each status code with an example).<br/>
**Answer :** **5 Main Categories of HTTP Status Codes :**<br/>
                **1.** Informational : 1xx<br/> 
                        **100 Continue:** This interim response indicates that the client should continue the request or ignore the response if the request is already finished. <br/>
                        **101 Switching Protocols:** This code is sent in response to an Upgrade request header from the client and indicates the protocol the server is switching to.<br/>
                        **102 Processing:** This code indicates that the server has received and is processing the request, but no response is available yet.<br/>
                        **103 Early Hints:** This status code is primarily intended to be used with the Link header, letting the user agent start preloading resources while the server prepares a response.<br/>
                **2.** Success : 2xx<br/>
                        **200 OK:** The request succeeded. The result meaning of "success" depends on the HTTP method.<br/>
                        **201 Created:** The request succeeded, and a new resource was created as a result. This is typically the response sent after POST requests, or some PUT requests.<br/>
                        **202 Accepted:** The request has been received but not yet acted upon. It is noncommittal, since there is no way in HTTP to later send an asynchronous response indicating the outcome of the request. It is intended for cases where another process or server handles the request, or for batch processing.<br/>
                        **203 Non-Authoritative Information:** This response code means the returned metadata is not exactly the same as is available from the origin server, but is collected from a local or a third-party copy. This is mostly used for mirrors or backups of another resource. Except for that specific case, the 200 OK response is preferred to this status.<br/>
                        **204 No Content:** There is no content to send for this request, but the headers may be useful. The user agent may update its cached headers for this resource with the new ones.<br/>
                **3.** Redirection : 3xx<br/>
                        **300 Multiple Choice:** The request has more than one possible response. The user agent or user should choose one of them. (There is no standardized way of choosing one of the responses, but HTML links to the possibilities are recommended so the user can pick.)<br/>
                        **301 Moved Permanently:** The URL of the requested resource has been changed permanently. The new URL is given in the response.<br/>
                        **302 Found:** This response code means that the URI of requested resource has been changed temporarily. Further changes in the URI might be made in the future. Therefore, this same URI should be used by the client in future requests.<br/>
                        **303 See Other:** The server sent this response to direct the client to get the requested resource at another URI with a GET request.<br/>
                        **304 Not Modified:** This is used for caching purposes. It tells the client that the response has not been modified, so the client can continue to use the same cached version of the response.<br/>
                **4.** Client Error : 4xx<br/>
                        **400 Bad Request:** The server cannot or will not process the request due to something that is perceived to be a client error (e.g., malformed request syntax, invalid request message framing, or deceptive request routing).<br/>
                        **401 Unauthorized:** Although the HTTP standard specifies "unauthorized", semantically this response means "unauthenticated". That is, the client must authenticate itself to get the requested response.<br/>
                        **402 Payment Required:** This response code is reserved for future use. The initial aim for creating this code was using it for digital payment systems, however this status code is used very rarely and no standard convention exists.<br/>
                        **403 Forbidden:** The client does not have access rights to the content; that is, it is unauthorized, so the server is refusing to give the requested resource. Unlike 401 Unauthorized, the client's identity is known to the server.<br/>
                        **404 Not Found:** The server can not find the requested resource. In the browser, this means the URL is not recognized. In an API, this can also mean that the endpoint is valid but the resource itself does not exist. Servers may also send this response instead of 403 Forbidden to hide the existence of a resource from an unauthorized client. This response code is probably the most well known due to its frequent occurrence on the web.<br/>
                        ***BONUS*** **418 I'm a Teapot:** The server refuses the attempt to brew coffee with a teapot.<br/>
                **5.** Server Error : 5xx<br/>
                        **500 Internal Server Error:** The server has encountered a situation it does not know how to handle.<br/>
                        **501 Not Implemented:** The request method is not supported by the server and cannot be handled. The only methods that servers are required to support (and therefore that must not return this code) are GET and HEAD.<br/>
                        **502 Bad Gateway:** This error response means that the server, while working as a gateway to get a response needed to handle the request, got an invalid response.<br/>
                        **503 Service Unavailable:** The server is not ready to handle the request. Common causes are a server that is down for maintenance or that is overloaded. Note that together with this response, a user-friendly page explaining the problem should be sent. This response should be used for temporary conditions and the Retry-After HTTP header should, if possible, contain the estimated time before the recovery of the service. The webmaster must also take care about the caching-related headers that are sent along with this response, as these temporary condition responses should usually not be cached.<br/>
                        **504 Gateway Timeout:** This error response is given when the server is acting as a gateway and cannot get a response in time.<br/>

**7.** What are the main components of HTTP requests and HTTP responses?<br/>
**Answer :** There are 3 main components. They are **1.** Status Line, **2.** Headers, and **3.** Body.<br/>

**8.** What are the main components of the HTTP request header and response header?<br/>
**Answer :** **HTTP Request Header:**<br/> 
                1. Type, Capabilities, and version of the browser that generates the request.<br/>
                2. OS used by client.<br/>
                3. Page That was requested. <br/>
                4. Various types of output accepted by the browser.<br/>
             **HTTP Response Header:**<br/>
                1. Type, Data, and Size of the file sent back by the server.<br/>
                2. Information regarding the server.<br/>

**9.** What is the difference between authentication and authorization?<br/>
**Answer :** In authentication process, the identity of users are checked for providing the access to the system. While in authorization process, person’s or user’s authorities are checked for accessing the resources. Authentication is done before the authorization process, whereas authorization process is done after the authentication process.<br/>

**10.** Briefly explain common API Authentication Methods.<br/>
**Answer :**  1. HTTP Basic Authentication : An HTTP user agent simply provides a username and password to prove their authentication. This approach does not require cookies, session IDs, login pages, and other such specialty solutions, and because it uses the HTTP header itself, there’s no need to handshakes or other complex response systems.<br/>
              2. API Keys : API Keys were created as somewhat of a fix to the early authentication issues of HTTP Basic Authentication and other such systems. In this approach, a unique generated value is assigned to each first time user, signifying that the user is known. When the user attempts to re-enter the system, their unique key (sometimes generated from their hardware combination and IP data, and other times randomly generated by the server which knows them) is used to prove that they’re the same user as before.<br/>
              3. OAuth : OAuth is not technically an authentication method, but a method of both authentication and authorization. When OAuth is used solely for authentication, it is what is referred to as “pseudo-authentication.” In this approach, the user logs into a system. That system will then request authentication, usually in the form of a token. The user will then forward this request to an authentication server, which will either reject or allow this authentication. From here, the token is provided to the user, and then to the requester. Such a token can then be checked at any time independently of the user by the requester for validation, and can be used over time with strictly limited scope and age of validity.