

- Security
-  SSLGetNegotiatedProtocolVersion(\_:\_:) Deprecated

Function

# SSLGetNegotiatedProtocolVersion(\_:\_:)

Obtains the negotiated protocol version of the active session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetNegotiatedProtocolVersion(
    _ context: SSLContext,
    _ protocol: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`protocol`  

On return, points to the negotiated protocol version of the active session. The value is set to SSLProtocol.sslProtocolUnknown if no SSL session is in progress.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

This function retrieves the version of the Secure Sockets Layer (SSL) or Transport Layer Security (TLS) protocol negotiated for the session. Note that the negotiated protocol may not be the same as your preferred protocol, depending on which protocol versions you enabled with the SSLSetProtocolVersionEnabled function. This function can return any of the following values:

- `kSSLProtocol2`

- `kSSLProtocol3`

- `kTLSProtocol1`

- `kSSLProtocolUnknown`

