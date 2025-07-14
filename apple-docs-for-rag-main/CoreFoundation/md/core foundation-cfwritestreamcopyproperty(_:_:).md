

- Core Foundation
-  CFWriteStreamCopyProperty(\_:\_:) 

Function

# CFWriteStreamCopyProperty(\_:\_:)

Returns the value of a property for a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamCopyProperty(
    _ stream: CFWriteStream!,
    _ propertyName: CFStreamPropertyKey!
) -> CFTypeRef!
```

## Parameters 

`stream`  

The stream to examine.

`propertyName`  

The name of the stream property to obtain. The available properties for standard Core Foundation streams are listed in Stream Properties.

## Return Value

The value of the property `propertyName`. Ownership follows the The Create Rule.

## Discussion

Each type of stream can define a set of properties that either describe or configure individual streams. A property can be any interesting information about a stream. Examples include the headers from an HTTP transmission, the expected number of bytes, file permission information, and so on. Use CFWriteStreamSetProperty(_:_:_:) to modify the value of a property, although some properties are read-only.

## See Also

### Examining Stream Properties

func CFWriteStreamCanAcceptBytes(CFWriteStream!) -> Bool

Returns whether a writable stream can accept new data without blocking.

func CFWriteStreamCopyError(CFWriteStream!) -> CFError!

Returns the error associated with a stream.

func CFWriteStreamGetError(CFWriteStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

func CFWriteStreamGetStatus(CFWriteStream!) -> CFStreamStatus

Returns the current state of a stream.

