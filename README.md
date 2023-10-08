# How-Web-Works-Exercise
Answer to subunit 15.1 exercise, contained in the readme file

## Part One: Solidify Terminology
In your own terms, define the following terms:
* **What is the HTTP?**
*   HTTP stands for "Hypertext Transfer Protocol" and is basically how websites communicate with servers
* **What is a URL?**
*  URL stands for "Uniform Resource Locator" and is basically an address that points to a website. It is composed of protocol, hostname, port, resource, and query.
* **What is DNS?**
*   DNS stands for "Domain Name System," and it takes hostnames and translates them to IP Addresses. This is how browsers know where to find an website from its URL.
* **What is a query string?**
*   A query string is additional information that is passed to the server from the browser. This additional information can be considered arguments, and multiple arguments may be passed at once. Sometimes JavaScript may use this information.
* **What are two HTTP verbs and how are they different?**
*   The two most common HTTP verbs are **_GET_** and **_POST_**, these both send requests but **_GET_** does so without any side effect such as changing server data, while **_POST_** will change data for purposes like sending mail, charging a credit card, making a post on social media...
  
| **_GET_**  | **_POST_** |
| ------------- | ------------- |
| No side effects  | side effects  |
| arguments passed in query string  | info sent in body  |
| Used for getting information according to arguments in query | Used for affecting some change, or sending data  |
| created when entering a URL in the browser, clicking links, and some form submissions  | used in _some_ form submissions, but **never** entering URL or clicking links  |

* **What is an HTTP request?**
*   An HTTP request is usually a request from the browser to the server for a webpage. Usually the first thing that is requested is the HTML page, but on that page there may be stylesheet and script references as well as image references, which will all require their own HTTP request as well.
* **What is an HTTP response?**
*   The HTTP response happens after the request, and usually contains the files that were requested. This starts as the html page of the website requested, but since the html usually contains style sheets and scripts and images, often there will be a seres of requests and responses to get those too following the main web site request.
* **What is an HTTP header? Gve a couple examples of request and response headers you have seen**
*   HTTP headers are used to request additional information, and in an http request they're used to suggest what the client would like, for example the request header "accept-language: fr" asks for a certain language, like French. An example of a response header would be "Date: Sun, 8 Oct 2023 22:34:00 GMT"

| **_Request Headers_**  | **_Response Headers_** |
| ------------- | ------------- |
| accept-language: [LANG]  | date: [DATE]  |

* **What are the processes that happen when you type “http://somesite.com/some/page.html” into a browser?**
*   first, "somesite.com" is turned into an IP Address, then the browser will connect to the IP address on a designated port (the default for HTTP is port 80). Then using HTTP protocol, the browser asks the server for the resources, in this case "/some/page.html". Lastly if there were a query string, it would be passed on as well.

