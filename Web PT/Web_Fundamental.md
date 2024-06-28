# **Web Fundamental Basic**  
## **HTTP Details**

**HTTP(HyperText Transfer Protocol):-** HTTP  is the set of rules used for communicating with web servers for the transmitting of webpage data, whether that is HTML, Images, Videos, etc.

**HTTPS (HyperText Transfer Protocol Secure):-** HTTPS is an extension of HTTP that adds a layer of security using SSL/TLS protocols to encrypt data transferred between clients and servers.

---

**URL:-** A URL (Uniform Resource Locator) is a unique identifier used to locate a resource on the Internet. It is also referred to as a web address.

<p align="center">
    <img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*cih496PZ5DyEubgfYUq3Zw.png" alt="Image Description" />
</p>

- **Scheme:-** This instructs on what protocol to use for accessing the resource such as HTTP, HTTPS, FTP (File Transfer Protocol).

- **User:-** Some services require authentication to log in, you can put a username and password into the URL to log in.

- **Host:-** The domain name or IP address of the server you wish to access.

- **Port:-** The Port that you are going to connect to, usually 80 for HTTP and 443 for HTTPS, but this can be hosted on any port between 1 - 65535.

- **Path:-** The file name or location of the resource you are trying to access.

- **Query String:-** Extra bits of information that can be sent to the requested path. 
 
    >**For example-** /blog?id=1 would tell the blog path that you wish to receive the blog article with the id of 1.

- **Fragment:-** This is a reference to a location on the actual page requested. This is commonly used for pages with long content and can have a certain part of the page directly linked to it, so it is viewable to the user as soon as they access the page.
---
**HTTP Method:-** An HTTP method, also known as an HTTP verb, is a standardized set of actions that define how clients (such as web browsers) communicate with servers (such as web servers) over the Hypertext Transfer Protocol (HTTP). 

<p align="center">
    <img src="https://storage.googleapis.com/dopingcloud/blog/en/2023/06/http-request-types.jpg.webp" alt="Image Description" />
</p>

- **GET Request:-** This is used for getting information from a web server.
  
- **POST Request:-** This is used for submitting data to the web server and potentially creating new records
  
- **PUT Request:-** This is used for submitting data to a web server to update information
  
- **DELETE Request:-** This is used for deleting information/records from a web server.
  
- **HEAD:-** The HEAD method in HTTP is similar to the GET method, It is often used to gather metadata about a resource, such as its size, content type, last-modified date, etc.
  
- **PATCH:-** The PATCH method in HTTP is used to apply partial modifications to a resource.
  
- **TRACE:-** It is used for the loopback of the request message, for testing or troubleshooting.

-----
**HTTP Requests:-** An HTTP request is a message sent by a client (such as a web browser or application) to a server, requesting to perform an action on a specific resource.

- The Request-line

- The analysis of source IP address, proxy and port

- The analysis of destination IP address, protocol, port and host

- The Requested URI (Uniform Resource Identifier)

- The Request method and Content

- The User-Agent header

- The Connection control header

- The Cache control header

 
 **For Example:**
</p>
<p align="center">
    <img src="https://www.oreilly.com/api/v2/epubs/9780596516680/files/httpatomoreillycomsourceoreillyimages2242227.png.jpg" alt="Image Description" />
</p>




