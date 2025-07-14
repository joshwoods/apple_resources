

- Security
-  SSLGetPeerID(\_:\_:\_:) Deprecated

Function

# SSLGetPeerID(\_:\_:\_:)

Retrieves the current peer ID data.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetPeerID(
    _ context: SSLContext,
    _ peerID: UnsafeMutablePointer,
    _ peerIDLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`peerID`  

On return, points to a buffer containing the peer ID data.

`peerIDLen`  

On return, the length of the peer ID data buffer.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

If the peer ID data for this context was not set by calling the SSLSetPeerID(_:_:_:) function, this function returns a `NULL` pointer in the `peerID` parameter, and `0` in the `peerIDLen` parameter.

