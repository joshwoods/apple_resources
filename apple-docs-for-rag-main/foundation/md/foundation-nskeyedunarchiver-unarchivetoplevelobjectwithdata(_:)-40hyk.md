

- Foundation
- NSKeyedUnarchiver
-  unarchiveTopLevelObjectWithData(\_:) 

Type Method

# unarchiveTopLevelObjectWithData(\_:)

Decodes a previously-archived object graph, and returns the root object.

iOS 9.0–12.0DeprecatediPadOS 9.0–12.0DeprecatedMac Catalyst 9.0–12.0DeprecatedmacOS 10.11–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0+watchOS 2.0–5.0DeprecatedSwift 4.0+

``` source
@nonobjc
class func unarchiveTopLevelObjectWithData(_ data: Data) throws -> Any?
```

## Parameters 

`data`  

An object graph previously encoded by NSKeyedArchiver.

## Return Value

The unarchived object, or `nil` if an error occurred.

## Discussion

This method throws an error if `data` does not contain valid keyed data.

## See Also

### Unarchiving Data

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

class func unarchiveObject(withFile: String) -> Any?

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` written to the file at a given path.

Deprecated

