

- Security
-  SSLGetSupportedCiphers(\_:\_:\_:) Deprecated

Function

# SSLGetSupportedCiphers(\_:\_:\_:)

Determines the values of the supported cipher suites.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetSupportedCiphers(
    _ context: SSLContext,
    _ ciphers: UnsafeMutablePointer,
    _ numCiphers: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`ciphers`  

On return, points to the values of the supported cipher suites. Before calling, you must allocate this buffer using the number of supported cipher suites retrieved from a call to the SSLGetNumberSupportedCiphers(_:_:) function.

`numCiphers`  

Points to the number of supported cipher suites that you want returned. Before calling, retrieve this value by calling the SSLGetNumberSupportedCiphers(_:_:) function.

## Return Value

A result code. See Secure Transport Result Codes. If the supplied buffer is too small, errSSLBufferOverflow is returned.

## Discussion

All the supported cipher suites are enabled by default. Use the SSLSetEnabledCiphers(_:_:_:) function to enable a subset of the supported cipher suites. Use the SSLGetEnabledCiphers(_:_:_:) function to determine which cipher suites are currently enabled.

