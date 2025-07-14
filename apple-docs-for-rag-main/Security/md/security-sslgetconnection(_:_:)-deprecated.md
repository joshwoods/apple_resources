

- Security
-  SSLGetConnection(\_:\_:) Deprecated

Function

# SSLGetConnection(\_:\_:)

Retrieves an I/O connection—such as a socket or endpoint—for a specific session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetConnection(
    _ context: SSLContext,
    _ connection: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`connection`  

On return, a pointer to a session connection reference. If no connection has been set using the SSLSetConnection(_:_:) function, then this parameter is `NULL` on return.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

You can use this function on either the client or server to retrieve the connection associated with a secure session.

