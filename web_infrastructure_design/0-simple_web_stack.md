A simple Web infrastructure/Stack contains an operating system (OS), a programming language, database software, and a Web server.

Let's look at the components of a Simple Web Infrastructure/Stack:

What is a server?

A server is a physical or virtual machine responsible for hosting and serving a website. It is a computer system or software that provides functionality or services to other computers, known as clients, over a network.
What is the role of the domain name?

The domain name (e.g., foobar.com) is a human-readable address used to access a website. It is translated into an IP address (e.g., 8.8.8.8) by the DNS system to locate the server.
What type of DNS record www is in www.foobar.com?

The www record is a CNAME (Canonical Name) DNS record, which points to the domain's primary record (foobar.com) or directly to the server.s IP address.
What is the role of the web server?

The webserver (Nginx) acts as a reverse proxy and web server. It receives HTTP requests from clients, forwards them to the application server if necessary, nd serves static content directly.
What is the role of the application server?

The application server executes the website's application logic, processing dynamic content requests, interacting with the database, and generating dynamic web pages.
What is the role of the database?

The database (MySQL) stores and manages the website's data, including user information, content, and settings.
What is the server using to communicate with the computer of the user requesting the website?

The server communicates with the user's computer over the Internet using the HTTP(S) protocol. When a user requests a webpage, their browser sends an HTTP request to the server, which responds with the requested webpage.

Some issues associated with running a simple web imfrastructure/stack include:

Single Point of Failure (SPOF): Since all components are hosted on a single server, any hardware or software failure can lead to complete website downtime.

Downtime when maintenance needed (like deploying new code web server needs to be restarted): Performing maintenance tasks such as deploying new code may require restarting the web server, causing temporary downtime for users accessing the website.

Scalability limitations: A simple web stack cannot scale if there is too much incoming traffic.The infrastructure may struggle to handle increased traffic as it's limited by the resources of a single server. Scaling horizontally (adding more servers) is not possible with this setup.

While the one-server web infrastructure serves the immediate needs of hosting the website, it presents several limitations in terms of reliability, scalability, and maintenance. To address these issues, considerations such as implementing redundancy, load balancing, and separating components onto different servers should be explored for a more robust and scalable solution.