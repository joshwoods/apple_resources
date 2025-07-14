

- Security
-  SSLWrite(\_:\_:\_:\_:) Deprecated

Function

# SSLWrite(\_:\_:\_:\_:)

Performs a typical application-level write operation.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLWrite(
    _ context: SSLContext,
    _ data: UnsafeRawPointer?,
    _ dataLength: Int,
    _ processed: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`data`  

A pointer to the buffer of data to write.

`dataLength`  

The amount, in bytes, of data to write.

`processed`  

On return, the length, in bytes, of the data actually written.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

The SSLWrite(_:_:_:_:) function might call the SSLWriteFunc function that you provide (see SSLSetIOFuncs(_:_:_:)). Because you may configure the underlying connection to operate in a no-blocking manner, a write operation might return `errSSLWouldBlock`, indicating that less data than requested was actually transferred. In this case, you should repeat the call to SSLWrite(_:_:_:_:) until some other result is returned.

