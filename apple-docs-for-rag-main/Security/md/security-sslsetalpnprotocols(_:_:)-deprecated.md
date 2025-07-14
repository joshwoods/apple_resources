

- Security
-  SSLSetALPNProtocols(\_:\_:) Deprecated

Function

# SSLSetALPNProtocols(\_:\_:)

Sets the list of supported applicaiton layer protocols.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15Deprecated

``` source
func SSLSetALPNProtocols(
    _ context: SSLContext,
    _ protocols: CFArray
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

The session context.

`protocols`  

An array of ASCII-encoded strings representing the supported protocols, such as `http/1.1`. See RFC 7301 for more details.

## Return Value

A result code. See Secure Transport Result Codes.

