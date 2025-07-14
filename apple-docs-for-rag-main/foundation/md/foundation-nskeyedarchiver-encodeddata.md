

- Foundation
- NSKeyedArchiver
-  encodedData 

Instance Property

# encodedData

The encoded data for the archiver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var encodedData: Data { get }
```

## Discussion

If encoding has not yet finished, invoking this property calls finishEncoding() and populates this property with the encoded data. If you initialized the keyed archiver with init(forWritingWith:) and a specific mutable data instance, this property contains that instance.

## See Also

### Archiving Data

class func archivedData(withRootObject: Any, requiringSecureCoding: Bool) throws -> Data

Encodes an object graph with the given root object into a data representation, optionally requiring secure coding.

func finishEncoding()

Instructs the receiver to construct the final data stream.

var outputFormat: PropertyListSerialization.PropertyListFormat

The format in which the receiver encodes its data.

var requiresSecureCoding: Bool

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

class func archivedData(withRootObject: Any) -> Data

Returns a data object that contains the encoded form of the object graph formed by the given root object.

Deprecated

class func archiveRootObject(Any, toFile: String) -> Bool

Archives an object graph rooted at a given object to a file at a given path.

Deprecated

