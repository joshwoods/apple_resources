

- Core Foundation
-  CFReadStreamGetBuffer(\_:\_:\_:) 

Function

# CFReadStreamGetBuffer(\_:\_:\_:)

Returns a pointer to a stream’s internal buffer of unread data, if possible.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamGetBuffer(
    _ stream: CFReadStream!,
    _ maxBytesToRead: CFIndex,
    _ numBytesRead: UnsafeMutablePointer!
) -> UnsafePointer!
```

## Parameters 

`stream`  

The stream to examine.

`maxBytesToRead`  

The maximum number of bytes to read. If greater than `0`, `maxBytesToRead` limits the number of bytes read; if `0` or less, all available bytes are read.

`numBytesRead`  

On return, contains the length of returned buffer. If `stream` is not open or has encountered an error, `numBytesRead` is set to `-1`.

## Return Value

A pointer to the internal buffer of unread data for `stream`, if possible; `NULL` otherwise. The buffer is good only until the next stream operation called on the stream. You should neither change the contents of the returned buffer nor attempt to deallocate the buffer; it is still owned by the stream. The bytes returned in the buffer are considered read from the stream.

## See Also

### Examining Stream Properties

func CFReadStreamCopyProperty(CFReadStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFReadStreamCopyError(CFReadStream!) -> CFError!

Returns the error associated with a stream.

func CFReadStreamGetError(CFReadStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

func CFReadStreamGetStatus(CFReadStream!) -> CFStreamStatus

Returns the current state of a stream.

func CFReadStreamHasBytesAvailable(CFReadStream!) -> Bool

Returns a Boolean value that indicates whether a readable stream has data that can be read without blocking.

