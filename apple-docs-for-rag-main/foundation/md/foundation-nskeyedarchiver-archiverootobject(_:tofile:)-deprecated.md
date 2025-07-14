

- Foundation
- NSKeyedArchiver
-  archiveRootObject(\_:toFile:) Deprecated

Type Method

# archiveRootObject(\_:toFile:)

Archives an object graph rooted at a given object to a file at a given path.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
class func archiveRootObject(
    _ rootObject: Any,
    toFile path: String
) -> Bool
```

Deprecated

Use +archivedDataWithRootObject:requiringSecureCoding:error: and -writeToURL:options:error: instead

## Parameters 

`rootObject`  

The root of the object graph to archive.

`path`  

The path of the file in which to write the archive.

## Return Value

true if the operation was successful, otherwise false.

## Discussion

This method archives the graph formed by the root object to a data object, then atomically writes it to the given path. The format of the archive is PropertyListSerialization.PropertyListFormat.binary.

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

var requiresSecureCoding: Bool

Indicates whether the archiver requires all archived classes to resist object substitution attacks.

class func archivedData(withRootObject: Any) -> Data

Returns a data object that contains the encoded form of the object graph formed by the given root object.

Deprecated

