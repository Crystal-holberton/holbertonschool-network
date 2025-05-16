# What happens when you type https://www.google.com in your browser and press Enter?
Initially it would seem like a simple answer, once you type google.com and hit enter googles front-page just appears on the screen. But much more than that happens behind the scenes.

In this file we will be looking at what actually happens in-between when you press that enter button.

## DNS Request:
After you press enter your computer sends a request to the domain name system (DNS) server which serves as an address book for all the domain names. This in turn sends back the exact IP address of the server pointed to.

## TCP/IP:
The computer establishes a connection with the server through the IP address. This connection is known as the Transmission Control Protocol (TCP) and this connection is able to establish this connection through the Internet Protocol (IP).

## Firewall:
A firewall checks the request you are making is allowed before permitting it to go through. This works both ways from the particular request from you one way and a similar check will be done back to finally be able to connect to the server.

## HTTPS/SSL:
After the connection is established your browser sends a request for the webpage using the encrytpion protocol Secure Sockets Layer (SSL) to encrypt the data that is shared between the computor and the server. This encryption is what makes the "S" in HTTPS implying that the connection is secure.

## Load-balancer:
Google is a large company with high traffic so to maintain this they implement a host of servers that use a laod-balancer to recieve most of the requests and send them to particular servers. The request will go through this load-balancer first and then forward it to the specific server depending on the algorithm.

## Web server:
The server that recieves the request will then send a response back to the load-balancer then it is forwarded back to your browser. This response is made up of the HTML, CSS and JavaScript files that make up Google's Homepage.

- HTML: tells the browser how to render the content of the page
- CSS: tells the browser how to style the content
- JavaScript: adds interactivity to the page

## Application server:
If some dynamic content is needed for Google search results then the web server will make the request to the application server.

## Database:
If the application server is needed, a request to the database server to get data may be used and sent back to the web server. The web server will then include this in the response back to the browser.

### Conclusion:
The page is then rendered on the browser and displayed to you.