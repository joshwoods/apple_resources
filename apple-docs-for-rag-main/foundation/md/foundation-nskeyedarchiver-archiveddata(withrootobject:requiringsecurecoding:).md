

- Foundation
- NSKeyedArchiver
-  archivedData(withRootObject:requiringSecureCoding:) 

Type Method

# archivedData(withRootObject:requiringSecureCoding:)

Encodes an object graph with the given root object into a data representation, optionally requiring secure coding.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func archivedData(
    withRootObject object: Any,
    requiringSecureCoding requiresSecureCoding: Bool
) throws -> Data
```

## Parameters 

`object`  

The root of the object graph to archive.

`requiresSecureCoding`  

A Boolean value indicating whether all encoded objects must conform to NSSecureCoding.

## Discussion

To prevent the possibility of encoding an object that NSKeyedUnarchiver can’t decode, set `requiresSecureCoding` to true whenever possible. This ensures that all encoded objects conform to NSSecureCoding.

Note

Enabling secure coding doesn’t change the output format of the archive. This means that you can encode archives with secure coding enabled, and decode them later with secure coding disabled.

## See Also

### Archiving Data

func finishEncoding()

Instructs the receiver to construct the final data stream.

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

