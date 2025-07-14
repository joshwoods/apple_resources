

- Security
-  SSLGetNegotiatedCipher(\_:\_:) Deprecated

Function

# SSLGetNegotiatedCipher(\_:\_:)

Retrieves the cipher suite negotiated for this session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetNegotiatedCipher(
    _ context: SSLContext,
    _ cipherSuite: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`cipherSuite`  

On return, points to the cipher suite that was negotiated for this session.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

You should call this function only when a session is active.

