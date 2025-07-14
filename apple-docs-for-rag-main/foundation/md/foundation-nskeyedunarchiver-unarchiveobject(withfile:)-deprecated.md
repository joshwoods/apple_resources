

- Foundation
- NSKeyedUnarchiver
-  unarchiveObject(withFile:) Deprecated

Type Method

# unarchiveObject(withFile:)

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` written to the file at a given path.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
class func unarchiveObject(withFile path: String) -> Any?
```

Deprecated

Use +unarchivedObjectOfClass:fromData:error: instead

## Parameters 

`path`  

A path to a file that contains an object graph previously encoded by `NSKeyedArchiver`.

## Return Value

The object graph previously encoded by `NSKeyedArchiver` written to the file `path`. Returns `nil` if there is no file at `path`.

## Discussion

This method raises an invalidArgumentException if the file at `path` does not contain a valid archive.

## See Also

### Unarchiving Data

class func unarchiveTopLevelObjectWithData(Data) throws -> Any?

Decodes a previously-archived object graph, and returns the root object.

static func unarchivedObject&lt;DecodedObjectType>(ofClass: DecodedObjectType.Type, from: Data) throws -> DecodedObjectType?

Decodes a previously-archived object graph, and returns the root object as the specified type.

class func unarchivedObject(ofClasses: Set&lt;AnyHashable>, from: Data) throws -> Any

Decodes a previously-archived object graph, returning the root object as one of the specified classes.

static func unarchivedObject(ofClasses: [AnyClass], from: Data) throws -> Any?

Decodes a previously-archived object graph, returning the root object as one of the specified classes.

var requiresSecureCoding: Bool

Indicates whether the receiver requires all unarchived classes to conform to NSSecureCoding.

class func unarchiveObject(with: Data) -> Any?

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` and stored in a given `NSData` object.

Deprecated

