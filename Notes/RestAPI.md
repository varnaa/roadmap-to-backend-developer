# REST API

---

#### REFER: [Understanding REST API](https://www.smashingmagazine.com/2018/01/understanding-using-rest-api/)


API stands for application programming interface. It allows developers to let two programs communicate with each other. For example, it allows a client to make a call to the server.

`An API is an application programming interface. It is a set of rules that allow programs to talk to each other. The developer creates the API on the server and allows the client to talk to it.`

#### Representational State Transfer (REST)
REST determines how an API looks like. It is a set of rules that developers follow when they create their API.

- Each URL is called a request while data sent back to you is called a response.

---

## The Anatomy Of A Request

- The endpoint
- The method 
- The headers
- The data / Body of the request

---

#### Endpoints
The endpoint (or route) is the url you request for. It follows this structure:

> root-endpoint/?

The root-endpoint is the starting point of the API you’re requesting from.
example: `https://api.github.com`

- The path determines the resources you're requesting for. You can access paths just like you can link to parts of a website. For example, to get a list of all posts tagged under “JavaScript” on Smashing Magazine, you navigate to `https://www.smashingmagazine.com/tag/javascript/` `https://www.smashingmagazine.com/` is the root-endpoint and `/tag/javascript` is the path.

- To understand what paths are available to you, you need to look through the API documentation. For example, let’s say you want to get a list of repositories by a certain user through Github’s API. The docs tells you to use the the following path to do so:

> /users/:username/repos

- Any colons (:) on a path denotes a variable. You should replace these values with actual values of when you send your request. In this case, you should replace :username with the actual username of the user you’re searching for. If I’m searching for my Github account, I’ll replace :username with zellwk.

- The final part of an endpoint is query parameters. Technically, query parameters are not part of the REST architecture, but you’ll see lots of APIs use them. So, to help you completely understand how to read and use API’s we’re also going to talk about them. Query parameters give you the option to modify your request with key-value pairs. They always begin with a question mark (?). Each parameter pair is then separated with an ampersand (&), like this:

> ?query1=value1&query2=value2

- Query parameters are usually added to your request when you need to modify the results given to you.

---

### The Method

The method is the type of request you send to the server. There are totally 5 types of requests:
- GET
- POST
- DELETE
- PUT
- PATCH

These methods provide meaning for the request you're making. They are used to perform four possible actions: `Create, Read, Update, Delete - (CRUD)`.


![Types of Methods](https://github.com/varnaa/roadmap-to-backend-developer/blob/master/screenshots/themethod.png)



---
