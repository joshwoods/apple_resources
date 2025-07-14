

- Core Foundation
-  CFReadStreamSetProperty(\_:\_:\_:) 

Function

# CFReadStreamSetProperty(\_:\_:\_:)

Sets the value of a property for a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamSetProperty(
    _ stream: CFReadStream!,
    _ propertyName: CFStreamPropertyKey!,
    _ propertyValue: CFTypeRef!
) -> Bool
```

## Parameters 

`stream`  

The stream to modify.

`propertyName`  

The name of the property to set. The available properties for standard Core Foundation streams are listed in CFStream.

`propertyValue`  

The value to which to set the property `propertyName` for `stream`. The allowed data type of the value depends on the property being set.

## Return Value

`TRUE` if `stream` recognizes and accepts the given property-value pair, otherwise`FALSE`.

## Discussion

Each type of stream can define a set of properties that either describe or configure individual streams. A property can be any interesting information about a stream. Examples include the headers from an HTTP transmission, the expected number of bytes, file permission information, and so on. Properties that can be set configure the behavior of the stream and may be modifiable only at particular times, such as before the stream has been opened. (In fact, you should assume that you can set properties only before opening the stream, unless otherwise noted.) To read the value of a property use CFReadStreamCopyProperty(_:_:), although some properties are write-only.

## See Also

### Setting Stream Properties

func CFReadStreamSetClient(CFReadStream!, CFOptionFlags, CFReadStreamClientCallBack!, UnsafeMutablePointer&lt;CFStreamClientContext>!) -> Bool

Assigns a client to a stream, which receives callbacks when certain events occur.

