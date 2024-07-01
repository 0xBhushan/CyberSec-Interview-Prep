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

----- 

**HTTP Response:-** An HTTP response is a message sent by a server to a client (such as a web browser or an application) in response to an HTTP request. 
- **Status Line:** The first line of an HTTP response is the status line, which includes: like- **HTTP Version, Status Code, Reason Phrase**
- **Headers:-** These provide additional information about the server's response, such as: **Content-Type, Content-Length, Date, Cache-Control, Server, Set-Cookie, etc.**
- **Blank Line:-** After the headers, there is a blank line that separates the headers from the optional message body. This line consists of only \r\n (carriage return followed by newline).
- **Message Body:-** Optionally, an HTTP response may include a message body. The content and format of the body depend on the request and response headers. For example:
  >For a GET request for an HTML page, the body would contain the HTML code.

  >For a POST request expecting JSON, the body might contain JSON data.
  
**For Example**

```
HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 145
Date: Wed, 28 Jun 2024 12:00:00 GMT

<!DOCTYPE html>
<html>
<head>
    <title>Example Page</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is an example response body.</p>
</body>
</html>
```
**Impotant**

- **Host:-** Specifies the domain name of the server (mandatory in HTTP/1.1).

- **User-Agent:-** Identifies the client making the request (e.g., browser name and version).

- **Content-Type-:** Specifies the media type of the request body (e.g., application/json, application/x-www-form-urlencoded).

- **Authorization:-** Contains credentials to authenticate the client with the server (e.g., tokens, API keys).

- **Accept:-** Indicates the media types accepted by the client for the response (e.g., text/html, application/json).
  
- **Set-Cookie:-** Information to store which gets sent back to the web server on each request (see cookies task for more information).

- **Cache-Control:-** How long to store the content of the response in the browser's cache before it requests it again.

- **Content-Type:-** This tells the client what type of data is being returned, i.e., HTML, CSS, JavaScript, Images, PDF, Video, etc.

- **Content-Encoding:-** What method has been used to compress the data to make it smaller when sending it over the internet.

-------

**HTTP Status Code:-** HTTP status codes are standard messages sent by a web server to a client's browser or application in response to a request. They tell the client if the request was successful, had an error, or needs additional action. These codes help in troubleshooting and understanding what happened during a web request.

**They are classified into 5 classes :**

- **1xx: Informational:–** Communicates transfer protocol-level information.
- **2xx: Success–** Indicates that the client’s request was accepted successfully.
- **3xx: Redirection:–** Indicates that the client must take some additional action in order to complete their request.
- **4xx: Client Error:–** This category of error status codes points the finger at clients.
- **5xx: Server Error:–** The server takes responsibility for these error status codes.

  
<p align="center">
    <img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*iBdspXxR_jjd-Yn7IDm43g.png" alt="Image Description" />
</p>
  
___

**Cookies:-** Cookies are small pieces of data stored on a user's device by a web browser while the user is browsing a website. They are used to remember stateful information or to track the user's browsing activity. 

 **There are two types of Cookies**
- **Session Cookies:-** Temporary cookies that expire when the user closes the browser. They are typically used for session management.

- **Persistent Cookies:-** Cookies with an expiration date set by the website. They remain on the user's device until they expire or are manually deleted.
  
  **For Example:-**

  > When you log into a website and choose "Remember Me", a persistent cookie might store your login credentials so you don't have to log in again each time you visit.

    > Online shopping websites use cookies to store items in your shopping cart across different pages or visits.
*********
## Domain Name System 
**DNS:-** DNS stands for Domain Name System. It is a fundamental technology used in the internet's infrastructure that translates domain names into IP addresses. Here’s a breakdown of its key components and functions:

- **Domain Names:-** These are human-readable addresses used to access websites (e.g., example.com). They are easier to remember than IP addresses.

- **IP Addresses:-** Every device connected to the internet is assigned a unique numerical label called an IP address (e.g., 192.0.2.1). IP addresses are used to identify and communicate with devices over the internet.

- **DNS Server:-** DNS servers are like internet directories that maintain a database of domain names and their corresponding IP addresses. When you type a domain name into your web browser, your computer queries a DNS server to find the corresponding IP address.
- **DNS Records:** These are entries within DNS databases that map domain names to IP addresses and provide other information about domain names, **such as** A (Address) Record, AAAA (IPv6 Address) Record, CNAME (Canonical Name) Record, MX (Mail Exchange) Record, TXT (Text) Record, NS (Name Server) Record, PTR (Pointer) Record etc..

- **Caching:-** DNS servers and clients often cache DNS records to speed up future queries and reduce network traffic.
- **Subdomains:-** Below the second-level domains, you can have additional levels of hierarchy known as subdomains. Subdomains allow for further organization and delegation within a domain. For example, in "blog.example.com," "blog" is a subdomain of "example.com".
- **Hostnames:-** Hostnames are specific names assigned to individual devices or services within a domain or subdomain. For instance, in "www.example.com," "www" is the hostname.
- **DNS Resolution Process:-** When you type a domain name (e.g., www.example.com) into your browser:

  > Your computer first checks its local DNS cache to see if it already knows the IP address for that domain.
  > 
  > If not found locally, your computer sends a query to a DNS resolver, typically operated by your Internet Service Provider (ISP) or a third-party DNS provider.
  > 
  >The DNS resolver checks its own cache. If the IP address is not cached, the resolver queries other DNS servers up the hierarchy until it finds the authoritative DNS server for that domain.
  >
  >The authoritative DNS server stores the official record (DNS zone file) for the domain and returns the corresponding IP address to the resolver.
  >
  >The resolver then returns the IP address to your computer, which can now connect to the desired website.
  
**For Example**
  <p align="center">
    <img src="https://almablog-media.s3.ap-south-1.amazonaws.com/007_d5abbba112.png" alt="Image Description" />
</p>

[For More Detils about DNS](https://www.almabetter.com/bytes/articles/what-is-dns)
---
