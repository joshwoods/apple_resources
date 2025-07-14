

- Foundation
- NSKeyedArchiver
-  finishEncoding() 

Instance Method

# finishEncoding()

Instructs the receiver to construct the final data stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func finishEncoding()
```

## Discussion

No more values can be encoded after this method is called. You must call this method when finished.

## See Also

### Related Documentation

init(forWritingWith: NSMutableData)

Initializes an archiver to encode data into a given a mutable-data object.

Deprecated

### Archiving Data

class func archivedData(withRootObject: Any, requiringSecureCoding: Bool) throws -> Data

Encodes an object graph with the given root object into a data representation, optionally requiring secure coding.

var encodedData: Data

The encoded data for the archiver.

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

