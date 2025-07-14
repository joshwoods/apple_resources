

- Security
-  SSLSetSessionConfig(\_:\_:) Deprecated

Function

# SSLSetSessionConfig(\_:\_:)

Sets a predefined configuration for the Secure Sockets Layer (SSL) session.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.15Deprecated

``` source
func SSLSetSessionConfig(
    _ context: SSLContext,
    _ config: CFString
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`config`  

The predefined configuration you want to apply to the SSL session. You can configure enabled protocol versions, enabled cipher suites, and the SSLSessionOption.fallback session option.

## Return Value

A result code. See Secure Transport Result Codes.

