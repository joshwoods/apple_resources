

- Security
-  SSLSetDatagramHelloCookie(\_:\_:\_:) Deprecated

Function

# SSLSetDatagramHelloCookie(\_:\_:\_:)

Sets the cookie value used in the Datagram Transport Layer Security (DTLS) hello message.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLSetDatagramHelloCookie(
    _ dtlsContext: SSLContext,
    _ cookie: UnsafeRawPointer?,
    _ cookieLen: Int
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`dtlsContext`  

The SSL context associated with the connection.

`cookie`  

The cookie value.

`cookieLen`  

The length of the cookie (up to 32 bytes).

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

This function should be called only on the server side, and is optional. The default cookie is a zero-length cookie.

