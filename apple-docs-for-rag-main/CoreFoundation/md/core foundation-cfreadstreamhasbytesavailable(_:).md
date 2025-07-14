

- Core Foundation
-  CFReadStreamHasBytesAvailable(\_:) 

Function

# CFReadStreamHasBytesAvailable(\_:)

Returns a Boolean value that indicates whether a readable stream has data that can be read without blocking.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamHasBytesAvailable(_ stream: CFReadStream!) -> Bool
```

## Parameters 

`stream`  

The stream to examine.

## Return Value

`TRUE` if data can be read from `stream` without blocking, otherwise `FALSE`. If `stream` cannot tell if data is available without actually trying to read the data, this function returns `TRUE`.

## See Also

### Examining Stream Properties

func CFReadStreamCopyProperty(CFReadStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFReadStreamGetBuffer(CFReadStream!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!) -> UnsafePointer&lt;UInt8>!

Returns a pointer to a stream’s internal buffer of unread data, if possible.

func CFReadStreamCopyError(CFReadStream!) -> CFError!

Returns the error associated with a stream.

func CFReadStreamGetError(CFReadStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

func CFReadStreamGetStatus(CFReadStream!) -> CFStreamStatus

Returns the current state of a stream.

