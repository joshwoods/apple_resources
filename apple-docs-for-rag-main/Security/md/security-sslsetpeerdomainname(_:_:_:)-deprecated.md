

- Security
-  SSLSetPeerDomainName(\_:\_:\_:) Deprecated

Function

# SSLSetPeerDomainName(\_:\_:\_:)

Specifies the fully qualified domain name of the peer.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLSetPeerDomainName(
    _ context: SSLContext,
    _ peerName: UnsafePointer?,
    _ peerNameLen: Int
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`peerName`  

The fully qualified domain name of the peer—for example, `store.apple.com`. The name is in the form of a C string, except that `NULL` termination is optional.

`peerNameLen`  

The number of bytes passed in the `peerName` parameter.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

You can use this function to verify the common name field in the peer’s certificate. If you call this function and the common name in the certificate does not match the value you specify in the `peerName` parameter, then handshake fails and returns `errSSLXCertChainInvalid`. Use of this function is optional.

This function can be called only when no session is active.

