 # Internet



## What is HTTP ?

HTTP is a protocol which allows the fetching of resources, such as HTML documents. It is the of foundation of any data exchange on the web and it is a client-server protocol. Which means requests are initiated by the recipient, usually the web browser.

#### Basic aspects of HTTP

- HTTP is simple, designed to be simple and human readable even with added complexity introduced in HTTP / 2.
- HTTP is extensible, HTTP headers make this protocol easy to extend and experiment with. New functionality can even be introduced by a simple agreement between a client and a server about a new header's semantics.
- HTTP is stateless but not sessionless. HTTP is stateless: there is no link between two requests being successively carried out on the same connection. This immediately has the prospect of being problematic for users attempting to interact with certain pages coherently, for example, using e-commerce shopping baskets. But while the core of HTTP itself is stateless, HTTP cookies allow the use of stateful sessions. Using header extensibility, HTTP Cookies are added to the workflow, allowing session creation on each HTTP request to share the same context, or the same state.



#### Query Parameters 

![A Quick Look into Path Parameters and Query Strings | LaptrinhX](https://cdn-images-1.medium.com/max/976/1*UTrozzGgca_LAgW11STH0Q.png)



#### Path Parameters

## ![Request Parameters | ServiceNow Developers](https://developer.servicenow.com/app_store_learnv2_rest_orlando_inbound_images_inbound_pathparms.png)



---

## Browsers and How they work ?

Browsers takes us to anywhere in the internet. It uses rendering engines to fetch the data such as images videos and documents.

## DNS and How it works?

The Domain Name System (DNS) is the phonebook of the Internet. Humans access information online through domain names, like nytimes.com or espn.com. Web browsers interact through Internet Protocol (IP) addresses. DNS translates domain names to IP address so browsers can load Internet resources.

Each device connected to the Internet has a unique IP address which other machines use to find the device. DNS servers eliminate the need for humans to memorize IP addresses such as 192.168.1.1 (in IPv4), or more complex newer alphanumeric IP addresses such as 2400:cb00:2048:1::c629:d7a2 (in IPv6).



4 components of DNS

- **[DNS recursor](https://www.cloudflare.com/learning/dns/dns-server-types#recursive-resolver)**- The recursor can be thought of as a librarian who is asked to go find a particular book somewhere in a library. The DNS recursor is a server designed to receive queries from client machines through applications such as web browsers. Typically the recursor is then responsible for making additional requests in order to satisfy the client’s DNS query.
- **Root nameserver**- The[root server](https://www.cloudflare.com/learning/dns/glossary/dns-root-server/)is the first step in translating (resolving) human readable host names into IP addresses. It can be thought of like an index in a library that points to different racks of books - typically it serves as a reference to other more specific locations.
- **[TLD nameserver](https://www.cloudflare.com/learning/dns/dns-server-types#tld-nameserver)**- The top level domain server (TLD) can be thought of as a specific rack of books in a library. This nameserver is the next step in the search for a specific IP address, and it hosts the last portion of a hostname (In example.com, the TLD server is “com”).
- **[Authoritative nameserver](https://www.cloudflare.com/learning/dns/dns-server-types#authoritative-nameserver)**- This final nameserver can be thought of as a dictionary on a rack of books, in which a specific name can be translated into its definition. The authoritative nameserver is the last stop in the nameserver query. If the authoritative name server has access to the requested record, it will return the IP address for the requested hostname back to the DNS Recursor (the librarian) that made the initial request.

#### The 8 steps in a DNS lookup:

1. A user types ‘example.com’ into a web browser and the query travels into the Internet and is received by a DNS recursive resolver.
2. The resolver then queries a DNS root nameserver (.).
3. The root server then responds to the resolver with the address of a Top Level Domain (TLD) DNS server (such as .com or .net), which stores the information for its domains. When searching for example.com, our request is pointed toward the .com TLD.
4. The resolver then makes a request to the .com TLD.
5. The TLD server then responds with the IP address of the domain’s nameserver, example.com.
6. Lastly, the recursive resolver sends a query to the domain’s nameserver.
7. The IP address for example.com is then returned to the resolver from the nameserver.
8. The DNS resolver then responds to the web browser with the IP address of the domain requested initially.
9. Once the 8 steps of the DNS lookup have returned the IP address for example.com, the browser is able to make the request for the web page:

10. The browser makes a [HTTP](https://www.cloudflare.com/learning/ddos/glossary/hypertext-transfer-protocol-http/) request to the IP address.
11. The server at that IP returns the webpage to be rendered in the browser (step 10).

## What is Domain Name ?

Domain name can be thought of as the human readable name of the ip address

## What is hosting ?

Ability to make an application available to the entire world ie Internet by hosting it in a server (PC ) and mapping the ip address of the server to a domain name and exposing this domain name to the users to interact with.

