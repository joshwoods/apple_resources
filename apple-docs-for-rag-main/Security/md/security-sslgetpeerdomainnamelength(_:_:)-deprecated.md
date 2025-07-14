

- Security
-  SSLGetPeerDomainNameLength(\_:\_:) Deprecated

Function

# SSLGetPeerDomainNameLength(\_:\_:)

Determines the length of a previously set peer domain name.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetPeerDomainNameLength(
    _ context: SSLContext,
    _ peerNameLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`peerNameLen`  

On return, points to the length of the peer domain name.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

If you previously called the SSLSetPeerDomainName(_:_:_:) function to specify a fully qualified domain name for the peer certificate, you can use the SSLGetPeerDomainName(_:_:_:) function to retrieve the peer domain name. Before doing so, you must call the SSLGetPeerDomainNameLength(_:_:) function to retrieve the buffer size needed for the domain name.

