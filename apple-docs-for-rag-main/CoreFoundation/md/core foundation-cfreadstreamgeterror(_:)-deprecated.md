

- Core Foundation
-  CFReadStreamGetError(\_:) Deprecated

Function

# CFReadStreamGetError(\_:)

Returns the error status of a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamGetError(_ stream: CFReadStream!) -> CFStreamError
```

Deprecated

Use CFReadStreamCopyError(_:) instead.

## Parameters 

`stream`  

The stream to examine.

## Return Value

The error status of `stream` returned in a CFStreamError structure.

## Discussion

The error field is `0` if no error has occurred. If the error field is not `0`, the `domain` field contains a code that identifies the domain in which the value of the `error` field should be interpreted.

## See Also

### Examining Stream Properties

func CFReadStreamCopyProperty(CFReadStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFReadStreamGetBuffer(CFReadStream!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!) -> UnsafePointer&lt;UInt8>!

Returns a pointer to a stream’s internal buffer of unread data, if possible.

func CFReadStreamCopyError(CFReadStream!) -> CFError!

Returns the error associated with a stream.

func CFReadStreamGetStatus(CFReadStream!) -> CFStreamStatus

Returns the current state of a stream.

func CFReadStreamHasBytesAvailable(CFReadStream!) -> Bool

Returns a Boolean value that indicates whether a readable stream has data that can be read without blocking.

