

- Security
-  SSLSetConnection(\_:\_:) Deprecated

Function

# SSLSetConnection(\_:\_:)

Specifies an I/O connection for a specific session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLSetConnection(
    _ context: SSLContext,
    _ connection: SSLConnectionRef?
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`connection`  

An SSL session connection reference. The connection data is opaque to Secure Transport; you can set it to any value that your application can use to uniquely identify the connection in the callback functions SSLReadFunc and SSLWriteFunc.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

You must establish a connection before creating a secure session. After calling the SSLCreateContext(_:_:_:) function to create an SSL session context, you call the SSLSetConnection(_:_:) function to specify the connection to which the context applies. You specify a value in the `connection` parameter that your callback routines can use to identify the connection. This value might be a pointer to a socket (if you are using the Sockets API) or an endpoint (if you are using Open Transport). For example, you might create a socket, start a connection on it, create a context reference, cast the socket to an SSLConnectionRef, and then pass both the context reference and connection reference to the SSLSetConnection(_:_:) function.

Note that the Sockets API is the preferred networking interface for new development.

On the client side, it’s assumed that communication has been established with the desired server on this connection. On the server side, it’s assumed that a connection has been established in response to an incoming client request .

This function must be called prior to the SSLHandshake(_:) function; consequently, this function can be called only when no session is active.

