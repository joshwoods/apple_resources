

- Security
-  SSLConnectionRef 

Type Alias

# SSLConnectionRef

A pointer to an opaque I/O connection object.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SSLConnectionRef = UnsafeRawPointer
```

## Discussion

The I/O connection object refers to data that identifies a connection. The connection data is opaque to Secure Transport; you can set it to any value that your application can use in the callback functions SSLReadFunc and SSLWriteFunc to uniquely identify the connection, such as a socket or endpoint. Use the SSLSetConnection(_:_:) function to assign a value to the connection object.

