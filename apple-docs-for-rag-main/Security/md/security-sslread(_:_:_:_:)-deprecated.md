

- Security
-  SSLRead(\_:\_:\_:\_:) Deprecated

Function

# SSLRead(\_:\_:\_:\_:)

Performs a normal application-level read operation.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLRead(
    _ context: SSLContext,
    _ data: UnsafeMutableRawPointer,
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

On return, points to the data read. You must allocate this buffer before calling the function. The size of this buffer must be equal to or greater than the value in the `dataLength` parameter.

`dataLength`  

The amount of data you would like to read.

`processed`  

On return, points to the number of bytes actually read.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

The SSLRead(_:_:_:_:) function might call the SSLReadFunc function that you provide (see SSLSetIOFuncs(_:_:_:). Because you may configure the underlying connection to operate in a nonblocking manner, a read operation might return `errSSLWouldBlock`, indicating that less data than requested was actually transferred. In this case, you should repeat the call to SSLRead(_:_:_:_:) until some other result is returned.

