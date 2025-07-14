

- Foundation
- NSKeyedArchiver
-  requiresSecureCoding 

Instance Property

# requiresSecureCoding

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var requiresSecureCoding: Bool { get set }
```

## Parameters 

`flag`  

true if the receiver requires NSSecureCoding; false if not.

## Discussion

If you set the archiver to require secure coding, it throws an exception if you attempt to archive a class which doesn’t conform to NSSecureCoding.

Note that the getter is on the superclass, NSCoder. See NSCoder for more information about secure coding.

Note

Enabling secure coding doesn’t change the output format of the archive. This means that you can encode archives with secure coding enabled, and decode them later with secure coding disabled.

## See Also

### Archiving Data

class func archivedData(withRootObject: Any, requiringSecureCoding: Bool) throws -> Data

Encodes an object graph with the given root object into a data representation, optionally requiring secure coding.

func finishEncoding()

Instructs the receiver to construct the final data stream.

var encodedData: Data

The encoded data for the archiver.

var outputFormat: PropertyListSerialization.PropertyListFormat

The format in which the receiver encodes its data.

class func archivedData(withRootObject: Any) -> Data

Returns a data object that contains the encoded form of the object graph formed by the given root object.

Deprecated

class func archiveRootObject(Any, toFile: String) -> Bool

Archives an object graph rooted at a given object to a file at a given path.

Deprecated

