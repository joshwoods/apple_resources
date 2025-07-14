

- Security
-  SSLGetPeerDomainName(\_:\_:\_:) Deprecated

Function

# SSLGetPeerDomainName(\_:\_:\_:)

Retrieves the peer domain name specified previously.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetPeerDomainName(
    _ context: SSLContext,
    _ peerName: UnsafeMutablePointer,
    _ peerNameLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`peerName`  

On return, points to the peer domain name.

`peerNameLen`  

A pointer to the length of the peer domain name. Before calling this function, retrieve the peer domain name length by calling the function SSLGetPeerDomainNameLength(_:_:).

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

If you previously called the SSLSetPeerDomainName(_:_:_:) function to specify a fully qualified domain name for the peer certificate, you can use the SSLGetPeerDomainName(_:_:_:) function to retrieve the domain name.

