

- Security
-  SSLSetEnabledCiphers(\_:\_:\_:) Deprecated

Function

# SSLSetEnabledCiphers(\_:\_:\_:)

Specifies a restricted set of SSL cipher suites to be enabled by the current SSL session context.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLSetEnabledCiphers(
    _ context: SSLContext,
    _ ciphers: UnsafePointer,
    _ numCiphers: Int
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`ciphers`  

A pointer to the cipher suites to enable.

`numCiphers`  

The number of cipher suites to enable.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

You can call this function, for example, to limit cipher suites to those that use exportable key sizes or to those supported by a particular protocol version.

This function can be called only when no session is active. The default set of enabled cipher suites is the complete set of supported cipher suites obtained by calling the SSLGetSupportedCiphers(_:_:_:) function.

Call the SSLGetEnabledCiphers(_:_:_:) function to determine which SSL cipher suites are currently enabled.

