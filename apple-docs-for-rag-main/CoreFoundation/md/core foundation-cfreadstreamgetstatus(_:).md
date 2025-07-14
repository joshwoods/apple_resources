

- Core Foundation
-  CFReadStreamGetStatus(\_:) 

Function

# CFReadStreamGetStatus(\_:)

Returns the current state of a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamGetStatus(_ stream: CFReadStream!) -> CFStreamStatus
```

## Parameters 

`stream`  

The stream to examine.

## Return Value

The current state of `stream`. See CFStreamStatus for the list of possible states.

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

func CFReadStreamHasBytesAvailable(CFReadStream!) -> Bool

Returns a Boolean value that indicates whether a readable stream has data that can be read without blocking.

