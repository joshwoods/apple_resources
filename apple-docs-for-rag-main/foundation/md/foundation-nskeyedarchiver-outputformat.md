

- Foundation
- NSKeyedArchiver
-  outputFormat 

Instance Property

# outputFormat

The format in which the receiver encodes its data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outputFormat: PropertyListSerialization.PropertyListFormat { get set }
```

## Discussion

The available formats are PropertyListSerialization.PropertyListFormat.xml and PropertyListSerialization.PropertyListFormat.binary.

## See Also

### Archiving Data

class func archivedData(withRootObject: Any, requiringSecureCoding: Bool) throws -> Data

Encodes an object graph with the given root object into a data representation, optionally requiring secure coding.

func finishEncoding()

Instructs the receiver to construct the final data stream.

var encodedData: Data

The encoded data for the archiver.

var requiresSecureCoding: Bool

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

class func archivedData(withRootObject: Any) -> Data

Returns a data object that contains the encoded form of the object graph formed by the given root object.

Deprecated

class func archiveRootObject(Any, toFile: String) -> Bool

Archives an object graph rooted at a given object to a file at a given path.

Deprecated

