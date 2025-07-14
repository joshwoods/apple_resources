

- Foundation
- PropertyListSerialization
-  writePropertyList(\_:to:format:options:error:) 

Type Method

# writePropertyList(\_:to:format:options:error:)

Writes a property list to the specified stream.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func writePropertyList(
    _ plist: Any,
    to stream: OutputStream,
    format: PropertyListSerialization.PropertyListFormat,
    options opt: PropertyListSerialization.WriteOptions,
    error: NSErrorPointer
) -> Int
```

## Parameters 

`plist`  

The property list that you want to write out.

`stream`  

An OutputStream instance that is open and ready to receive the property list data.

`format`  

One of the property list formats defined in PropertyListSerialization.PropertyListFormat.

`opt`  

Currently unused. Set to `0`.

`error`  

A pointer that the function may set to an NSError object when an error occurs to provide additional information about the error.

## Return Value

The number of bytes written to the stream. A return value of `0` indicates that an error occurred.

## See Also

### Serializing a Property List

class func data(fromPropertyList: Any, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions) throws -> Data

Returns an `NSData` object containing a given property list in a specified format.

typealias WriteOptions

