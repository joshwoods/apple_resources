

- Security
-  SSLCopyRequestedPeerName(\_:\_:\_:) Deprecated

Function

# SSLCopyRequestedPeerName(\_:\_:\_:)

Determines the buffer size needed for the peer domain name.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.15Deprecated

``` source
func SSLCopyRequestedPeerName(
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

The fully qualified domain name of the peer—for example, `store.apple.com`. The name is in the form of a C string, except that `NULL` termination is optional.

`peerNameLen`  

On return, points to the length of the peer domain name.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

Use the `peerNameLen` returned by this function when calling the SSLCopyRequestedPeerNameLength(_:_:) function.

