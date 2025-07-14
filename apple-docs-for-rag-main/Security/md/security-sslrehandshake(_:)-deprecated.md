

- Security
-  SSLReHandshake(\_:) Deprecated

Function

# SSLReHandshake(\_:)

Requests renegotiation of the SSL handshake. Server only.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.15Deprecated

``` source
func SSLReHandshake(_ context: SSLContext) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

On success, call the SSLHandshake(_:) function or the SSLRead(_:_:_:_:) function, or both, as appropriate, as you would for the original handshake.

