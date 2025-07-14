

- Security
-  SSLReadFunc 

Type Alias

# SSLReadFunc

A pointer to a customized read function that secure transport calls to read data from the connection.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SSLReadFunc = (SSLConnectionRef, UnsafeMutableRawPointer, UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`connection`  

A connection reference.

`data`  

On return, your callback should overwrite the memory at this location with the data read from the connection.

`dataLength`  

On input, a pointer to an integer representing the length of the data in bytes. On return, your callback should overwrite that integer with the number of bytes actually transferred.

## Return Value

Your callback must return an appropriate result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

Before using the secure transport API, you must create a read function (conforming to the SSLReadFunc prototype) and a write function (conforming to the SSLWriteFunc prototype) and provide them to the library by calling the SSLSetIOFuncs(_:_:_:) function.

You may configure the underlying connection to operate in a non-blocking manner; in that case, a read operation may well return errSSLWouldBlock, indicating less data than requested was transferred and nothing is wrong except that the requested I/O hasn’t completed. This result is returned to the caller from the functions SSLRead(_:_:_:_:), SSLWrite(_:_:_:_:), or SSLHandshake(_:).

