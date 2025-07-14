

- Security
-  SSLGetProtocolVersionMax(\_:\_:) Deprecated

Function

# SSLGetProtocolVersionMax(\_:\_:)

Gets the maximum protocol version allowed by the application for a given SSL context.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLGetProtocolVersionMax(
    _ context: SSLContext,
    _ maxVersion: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

The SSL context associated with the connection.

`maxVersion`  

The address of an SSLProtocol integer where the maximum version should be stored. See SSLProtocol for a list of possible values.

## Return Value

A result code. See Secure Transport Result Codes.

