

- Security
-  SSLGetBufferedReadSize(\_:\_:) Deprecated

Function

# SSLGetBufferedReadSize(\_:\_:)

Determines how much data is available to be read.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetBufferedReadSize(
    _ context: SSLContext,
    _ bufferSize: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`bufferSize`  

On return, the size of the data to be read.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

This function determines how much data you can be guaranteed to obtain in a call to the SSLRead(_:_:_:_:) function. This function does not block or cause any low-level read operations to occur.

