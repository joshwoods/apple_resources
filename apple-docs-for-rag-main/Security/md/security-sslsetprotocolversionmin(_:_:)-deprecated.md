

- Security
-  SSLSetProtocolVersionMin(\_:\_:) Deprecated

Function

# SSLSetProtocolVersionMin(\_:\_:)

Sets the minimum protocol version allowed by the application for a given SSL context.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLSetProtocolVersionMin(
    _ context: SSLContext,
    _ minVersion: SSLProtocol
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

The SSL context associated with the connection.

`minVersion`  

The new minimum version (SSLProtocol.tlsProtocol1, for example). See SSLProtocol for a complete list.

## Return Value

A result code. See Secure Transport Result Codes.

