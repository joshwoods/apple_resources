

- Security
- Secure Transport
-  Using the Secure Socket Layer for Network Communication 

Article

# Using the Secure Socket Layer for Network Communication

Establish Secure Sockets Layer (SSL) sessions to facilitate secure communication between client and server.

## Overview

The following terms are used in this discussion:

Client  
The initiator of an SSL session. The canonical example of a client is a web browser communicating with an HTTPS URL.

Server  
An entity that accepts requests for SSL sessions made by clients. An example is a secure web server.

SSLSession  
An entity whose existence is bounded by calls to the functions SSLHandshake(_:) and SSLClose(_:). An active session is in some state between these two calls, inclusive.

SSLSessionContext  
The state associated with one session. A session context cannot be reused for multiple sessions.

Most applications need only a few of the functions in this API, which are normally called in the following sequence:

- Prepare for a session

- Call SSLCreateContext(_:_:_:) to create a new SSL session context.

- Write the SSLWriteFunc and SSLReadFunc I/O functions and register them with Secure Transport by calling the SSLSetIOFuncs(_:_:_:) function.

- Establish a connection using CFNetwork, BSD Sockets, or Open Transport. Then call SSLSetConnection(_:_:) to specify the connection to which the SSL session context applies.

- Call SSLSetPeerDomainName(_:_:_:) to specify the fully-qualified domain name of the peer to which you want to connect (optional but highly recommended).

- Call SSLSetCertificate(_:_:) to specify the certificate to be used in authentication (required for server side, optional for client).

- Start a session

- Call SSLHandshake(_:) to perform the SSL handshake and establish a secure session.

- Maintain a session

- To transfer data over the secure session, Secure Transport calls your SSLWrite(_:_:_:_:) and SSLRead(_:_:_:_:) functions as needed.

- End a session

- Call SSLClose(_:) to close the secure session.

- Close the connection and dispose of the connection reference.

- Release the SSL session context by calling CFRelease.

- If you called `SSLGetPeerCertificates` to obtain any certificates, call CFRelease to release the certificate reference objects.

In many cases, it is easier to use the CFNetwork API than Secure Transport to implement a simple connection to a secure (HTTPS) URL. See CFNetwork Programming Guide for documentation of the CFNetwork API and the CFNetworkHTTPDownload sample code for an example of code that downloads data from a URL. If you specify an HTTPS URL, this routine automatically uses Secure Transport to encrypt the data stream.

For functions to manage and evaluate certificates, see Certificate, Key, and Trust Services.

