

- Security
-  SSLWriteFunc 

Type Alias

# SSLWriteFunc

A pointer to a customized write function that secure transport calls to write data to the connection.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SSLWriteFunc = (SSLConnectionRef, UnsafeRawPointer, UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`connection`  

The SSL session connection reference.

`data`  

A pointer to the data to write to the connection.You must allocate this memory before calling this function.

`dataLength`  

Before calling, an integer representing the length of the data in bytes. On return, this is the number of bytes actually transferred.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

Before using the secure transport API, you must write the functions SSLReadFunc and SSLWriteFunc and provide them to the library by calling the SSLSetIOFuncs(_:_:_:) function.

You may configure the underlying connection to operate in a non-blocking manner. In that case, a write operation may well return errSSLWouldBlock, indicating less data than requested was transferred and nothing is wrong except that the requested I/O hasn’t completed. This result is returned to the caller from the functions SSLRead(_:_:_:_:), SSLWrite(_:_:_:_:), or SSLHandshake(_:).

