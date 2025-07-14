

- Security
-  SSLCopyRequestedPeerNameLength(\_:\_:) Deprecated

Function

# SSLCopyRequestedPeerNameLength(\_:\_:)

Obtains the hostname specified by the client in the ServerName extension (SNI). Server only.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.15Deprecated

``` source
func SSLCopyRequestedPeerNameLength(
    _ ctx: SSLContext,
    _ peerNameLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`ctx`  

An SSL session context reference.

`peerNameLen`  

The length of the peer name, as retrieved by calling the SSLCopyRequestedPeerName(_:_:_:) function.

## Return Value

A result code. See Secure Transport Result Codes.

