

- Security
-  SSLGetNumberSupportedCiphers(\_:\_:) Deprecated

Function

# SSLGetNumberSupportedCiphers(\_:\_:)

Determines the number of cipher suites supported.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetNumberSupportedCiphers(
    _ context: SSLContext,
    _ numCiphers: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`numCiphers`  

On return, points to the number of supported cipher suites.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

You use the number of enabled cipher suites returned by this function when you call the SSLGetNumberSupportedCiphers(_:_:) function to retrieve the list of currently enabled cipher suites.

