

- Foundation
- NSKeyedArchiver
-  archivedData(withRootObject:) Deprecated

Type Method

# archivedData(withRootObject:)

Returns a data object that contains the encoded form of the object graph formed by the given root object.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
class func archivedData(withRootObject rootObject: Any) -> Data
```

Deprecated

Use +archivedDataWithRootObject:requiringSecureCoding:error: instead

## Parameters 

`rootObject`  

The root of the object graph to archive.

## Return Value

An `NSData` object containing the encoded form of the object graph whose root object is `rootObject`. The format of the archive is PropertyListSerialization.PropertyListFormat.binary.

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

class func archiveRootObject(Any, toFile: String) -> Bool

Archives an object graph rooted at a given object to a file at a given path.

Deprecated

