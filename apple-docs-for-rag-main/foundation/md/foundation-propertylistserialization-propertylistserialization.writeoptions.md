

- Foundation
- PropertyListSerialization
-  PropertyListSerialization.WriteOptions 

Type Alias

# PropertyListSerialization.WriteOptions

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias WriteOptions = Int
```

## See Also

### Serializing a Property List

class func data(fromPropertyList: Any, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions) throws -> Data

Returns an `NSData` object containing a given property list in a specified format.

class func writePropertyList(Any, to: OutputStream, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions, error: NSErrorPointer) -> Int

Writes a property list to the specified stream.

