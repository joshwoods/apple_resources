

- Core Foundation
-  CFReadStreamCopyProperty(\_:\_:) 

Function

# CFReadStreamCopyProperty(\_:\_:)

Returns the value of a property for a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamCopyProperty(
    _ stream: CFReadStream!,
    _ propertyName: CFStreamPropertyKey!
) -> CFTypeRef!
```

## Parameters 

`stream`  

The stream to examine.

`propertyName`  

The name of the stream property to obtain. The available properties for standard Core Foundation streams are listed in CFStream.

## Return Value

The value of the property `propertyName`. Ownership follows the The Create Rule.

## Discussion

Each type of stream can define a set of properties that either describe or configure individual streams. A property can be any information about a stream, other than the actual data the stream handles. Examples include the headers from an HTTP transmission, the expected number of bytes, file permission information, and so on. Use CFReadStreamSetProperty(_:_:_:) to modify the value of a property, although some properties are read-only.

## See Also

### Examining Stream Properties

func CFReadStreamGetBuffer(CFReadStream!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!) -> UnsafePointer&lt;UInt8>!

Returns a pointer to a stream’s internal buffer of unread data, if possible.

func CFReadStreamCopyError(CFReadStream!) -> CFError!

Returns the error associated with a stream.

func CFReadStreamGetError(CFReadStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

func CFReadStreamGetStatus(CFReadStream!) -> CFStreamStatus

Returns the current state of a stream.

func CFReadStreamHasBytesAvailable(CFReadStream!) -> Bool

Returns a Boolean value that indicates whether a readable stream has data that can be read without blocking.

