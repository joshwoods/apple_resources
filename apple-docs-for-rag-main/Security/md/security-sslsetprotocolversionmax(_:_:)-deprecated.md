

- Security
-  SSLSetProtocolVersionMax(\_:\_:) Deprecated

Function

# SSLSetProtocolVersionMax(\_:\_:)

Sets the maximum protocol version allowed by the application for a given SSL context.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLSetProtocolVersionMax(
    _ context: SSLContext,
    _ maxVersion: SSLProtocol
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

The SSL context associated with the connection.

`maxVersion`  

The new maximum version (SSLProtocol.tlsProtocol1, for example). See SSLProtocol for a complete list.

## Return Value

A result code. See Secure Transport Result Codes.

