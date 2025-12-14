TryHackMe — DNS in Detail
🎯 Objective

This room provides an in-depth understanding of the Domain Name System (DNS) by explaining its core concepts, architecture, and functionality in detail.

 Key Concepts Learned

Hierarchical structure and workflow of DNS

Different types of DNS servers and their roles

Common DNS record types and their purposes

 Tools Used

nslookup: Used within the built-in virtual lab to query domain names, subdomains, and DNS records for information gathering and analysis.

📌 Important Takeaways

In this room, I gained a clear understanding of how DNS works behind the scenes when a user searches for a domain such as google.com. The DNS resolution process begins with the Root DNS server, which acts as the backbone of the internet by identifying the requested top-level domain (TLD) and forwarding the query to the appropriate TLD server.

The TLD server stores information about the authoritative DNS servers responsible for a specific domain. Each domain typically has at least one primary authoritative server along with a backup for redundancy. The authoritative DNS server contains the actual DNS records for the domain and responds with the requested record type.

This information is then returned to the recursive DNS server, which caches the result locally to improve performance for future requests before sending the response back to the client.

The room also clarified my understanding of subdomains, including the fact that a single domain can have multiple subdomains. I learned that the maximum length of a subdomain label is 63 characters, while the total maximum length of a fully qualified domain name is 253 characters.

Additionally, I explored various DNS record types such as A, AAAA, CNAME, MX, and TXT, understanding their individual purposes and how they are used in real-world DNS configurations.

Learning DNS is essential for ethical hacking, as a solid understanding of domain names and subdomains is critical for effective reconnaissance. Without this knowledge, it becomes difficult to analyze backend systems or understand how IP addresses are resolved into domain names.

 Skills Improved

DNS fundamentals and architecture

DNS enumeration using nslookup
