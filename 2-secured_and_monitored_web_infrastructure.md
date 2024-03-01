A Secured and Monitored Web Infrastucture is a three-server web infrastructure that is secured, monitored, and serves encrypted traffic. It is made up of the combination of technical and administrative measures put in place to ensure the security and reliability of a website or online service.
Firewalls: Added for security to control and filter network traffic, preventing unauthorized access and mitigating potential threats.

SSL Certificate for HTTPS: This enables encryption of data transmitted between clients and the website, safeguarding sensitive information from interception or manipulation.

Monitoring Clients: These are essential for tracking the performance, availability, and security of the infrastructure in real-time, allowing administrators to proactively identify and address issues.

What are firewalls for? A firewall is a network security device that plays a crucial role in safeguarding computer networks. Let’s explore what firewalls do and why they are essential:

Incoming and Outgoing Traffic: Firewalls monitor both incoming and outgoing network traffic.
Authorized vs. Unwanted Traffic: They allow authorized traffic (such as legitimate requests) while blocking unwanted or potentially harmful traffic.
Unauthorized Access Prevention: Firewalls protect against unauthorized access attempts by outsiders.
Filtering: Firewalls act as gatekeepers, filtering traffic between your computer and external networks (like the internet).
Traffic Validation: They assess network traffic for anything malicious, ensuring only valid requests pass through.
Malware Defense: Firewalls guard against malware attempting to infiltrate your system.
Data Protection: They prevent sensitive data from leaving your network.
Security: Firewalls protect against unauthorized access, malware, and cyber threats.
Privacy: They prevent data leaks and ensure sensitive information stays within your network.
Network Integrity: Firewalls maintain the integrity of your network by controlling traffic flow. A well-configured firewall is your first line of defense against potential security risks.
Why is traffic served over HTTPS?

Traffic is served over HTTPS to protect users information. HTTPS encrypts data transmitted between clients and the website, protecting sensitive information such as login credentials, payment details, and personal data from unauthorized access or interception. It ensures data confidentiality and integrity, enhancing the security of the communication channel.
What is monitoring used for?

Monitoring is used to track the health, performance, and security of the infrastructure and applications. It provides real-time insights into resource utilization, system errors, security incidents, and performance bottlenecks, enabling administrators to detect and address issues promptly.
How does monitoring tools collect data?

Monitoring tools collect data through monitoring clients or agents installed on servers, applications, and network devices. These clients continuously gather metrics, logs, and events from the monitored components and transmit them to a centralized monitoring platform for analysis and visualization.

Terminating SSL at the load balancer level: Terminating SSL at the load balancer exposes decrypted traffic within the internal network, increasing the risk of data exposure if the load balancer is compromised. It's generally recommended to terminate SSL at the application servers to maintain end-to-end encryption.

Having a single MySQL server capable of accepting writes: Having only one MySQL server capable of accepting writes creates a single point of failure. If the server fails, write operations will be disrupted, impacting the availability and integrity of the database. Implementing MySQL replication or clustering can provide redundancy and fault tolerance.

Having Uniformity of server components: Having servers with identical components (database, web server, application server) may lead to homogeneity, making the infrastructure vulnerable to widespread failures or security breaches. Introducing diversity in server configurations and components can enhance resilience and mitigate risks associated with common vulnerabilities.