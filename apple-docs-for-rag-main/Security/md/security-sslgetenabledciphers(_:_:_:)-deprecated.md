

- Security
-  SSLGetEnabledCiphers(\_:\_:\_:) Deprecated

Function

# SSLGetEnabledCiphers(\_:\_:\_:)

Determines which SSL cipher suites are currently enabled.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetEnabledCiphers(
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

On return, points to the enabled cipher suites. Before calling, you must allocate this buffer using the number of enabled cipher suites retrieved from a call to the SSLGetNumberEnabledCiphers(_:_:) function.

`numCiphers`  

Pointer to the number of enabled cipher suites. Before calling, retrieve this value by calling the SSLGetNumberEnabledCiphers(_:_:) function.

## Return Value

A result code. See Secure Transport Result Codes. If the supplied buffer is too small, errSSLBufferOverflow is returned.

## Discussion

Call the SSLSetEnabledCiphers(_:_:_:) function to specify which SSL cipher suites are enabled.

