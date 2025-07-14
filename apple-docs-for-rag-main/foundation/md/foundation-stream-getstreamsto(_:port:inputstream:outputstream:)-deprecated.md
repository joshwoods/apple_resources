

- Foundation
- Stream
-  getStreamsTo(\_:port:inputStream:outputStream:) Deprecated

Type Method

# getStreamsTo(\_:port:inputStream:outputStream:)

Creates and returns by reference an `NSInputStream` object and `NSOutputStream` object for a socket connection with a given host on a given port.

macOS 10.3–10.10Deprecated

``` source
class func getStreamsTo(
    _ host: Host,
    port: Int,
    inputStream: AutoreleasingUnsafeMutablePointer?,
    outputStream: AutoreleasingUnsafeMutablePointer?
)
```

Deprecated

Use nw_connection_t in Network framework instead

## Parameters 

`host`  

The host to which to connect.

`port`  

The port to connect to on `host`.

`inputStream`  

Upon return, contains the input stream. If `nil` is passed, the stream object is not created.

`outputStream`  

Upon return, contains the output stream. If `nil` is passed, the stream object is not created.

## Discussion

If neither `port` nor `host` is properly specified, no socket connection is made.

## See Also

### Related Documentation

Stream Programming Guide

