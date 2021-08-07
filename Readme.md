# History of HTTP

Invented by Tim Berners-Lee at CERN in the years 1989–1991, HTTP (Hypertext Transfer Protocol) is the underlying communication protocol of World Wide Web. 
HTTP functions as a request–response protocol in the client–server computing model. HTTP standards are developed by the Internet Engineering Task Force (IETF) 
and the World Wide Web Consortium (W3C), culminating in the publication of a series of Requests for Comments (RFCs). HTTP has four versions — HTTP/0.9, HTTP/1.0, 
HTTP/1.1, and HTTP/2.0. Today the version in common use is HTTP/1.1 and the future will be HTTP/2.0.

## HTTP/0.9 — The One-line Protocol -
1.Initial version of HTTP — a simple client-server, request-response, telenet-friendly protocol
2.Request nature: single-line (method + path for requested document)
3.Methods supported: GET only
4.Response type: hypertext only
5.Connection nature: terminated immediately after the response
6.No HTTP headers (cannot transfer other content type files), No status/error codes, No URLs, No versioning

## HTTP/1.0 — Building extensibility -
1.Browser-friendly protocol
2.Provided header fields including rich metadata about both request and response (HTTP version number, status code, content type)
3.Response: not limited to hypertext (Content-Type header provided ability to transmit files other than plain HTML files — e.g. scripts, stylesheets, media)
4.Methods supported: GET , HEAD , POST
5.Connection nature: terminated immediately after the response

## Establishing a new connection for each request — major problem in both HTTP/0.9 and HTTP/1.0
Both HTTP/0.9 and HTTP/1.0 required to open up a new connection for each request (and close it immediately after the response was sent). 
Each time a new connection establishes, a TCP three-way handshake should also occur. For better performance, it was crucial to reduce these round-trips 
between client and server. HTTP/1.1 solved this with persistent connections.

## HTTP/1.1 — The standardized protocol -
1.This is the HTTP version currently in common use.
2.Introduced critical performance optimizations and feature enhancements — persistent and pipelined connections, chunked transfers, compression/decompression, 
  content negotiations, virtual hosting (a server with a single IP Address hosting multiple domains), faster response and great bandwidth savings by adding cache support.
3.Methods supported: GET , HEAD , POST , PUT , DELETE , TRACE , OPTIONS
4.Connection nature: long-lived

## HTTPS -
1.Hyper Text Transfer Protocol Secure (HTTPS) is the secure version of HTTP. It uses SSL/TLS for secure encrypted communications.
2.Originally developed by Netscape in mid-1990s, SSL (Secure Socket Layer) is a cryptographic protocol enhancement to HTTP, which defines how client and server 
  should communicate with each other securely. TLS (Transport Layer Security) is the successor of SSL.
3.An HTTPS connection can protect the data transfer from the man-in-the-middle attacks and common security threats by providing bidirectional encryption for 
  communications between a client and server.

