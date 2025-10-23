PART-A : Browser-Analysis

1). According to the observations I made, the request header of HTTP did not contain any cookies, while the HTTPS one did. Host was not found in request header of HTTPS, but was found in HTTP. Also, the sec fetch site was same origin for HTTPS while cross-site for HTTP.This means that, the HTTPS webiste is requesting data from the same origin, but from a different page while HTTP website is requesting data from a completely different website.

Yes, the actual data can be seen in both HTTP and HTTPS. But in HTTP, anyone monitoring the network other than the client and server can also see the data as there is no encryption. In HTTP, the actual data is encrypted, but the dev tools decrypt it and shows us and hence we are able to see it.

HTTPS is more secure than HTTP becuase HTTPS encrypts the data, so only the client and the server will be able to see headers,URL’s,contents etc. Whereas HTTP sends data as plain text, so anyone on the network like the internet service provider,network admin or other users using the same wifi can access the data.Hence HTTPS is more secure than HTTP.

2). For NeverSSL, only 2 requests were made(the online/ and favicon.ico requests). The online/ request header recieved html file as response, while favicon.ico recieved an image represented as a matrix as response. For github, around 168 requests were made which included requests for images, javascript files, stylesheets and gif. For youtube, around 95 requests were made for images, gif’s,stylesheets,fetch and xhr. Github made the most requests as it loads even samll files like images and icons unlike youtube which loads it in big bundles(so it requires lesser requests).

3). Load time for all websites:

	NeverSSL  - 6.11 s
	
	Github       - 3.03 s
	
	YouTube    - 36.58 s
	
    The online/ request of NeverSSL took the longest.
	
DNS lookup time – DNS is basically a server that acts like a phonebook. It takes human readable domain names and returns the corresponding IP address associated with that particular domain name, to our browser.Then our browser connects to the server using this address and loads the website. DNS lookup time, is the time taken by browser to convert domain name to its corresponding IP address. 

Connection time -  Connection time is the time required to make a secure connection between the client and the server including handshakes and encryption of data.

TTFB – After the browser sends request, the total time taken to recieve the first byte of data from the server is called TTFB(time to first byte). It involves request time, response time,  DNS lookup, connection timeand server processing time.
