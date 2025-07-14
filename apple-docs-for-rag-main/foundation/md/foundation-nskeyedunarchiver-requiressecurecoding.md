

- Foundation
- NSKeyedUnarchiver
-  requiresSecureCoding 

Instance Property

# requiresSecureCoding

Indicates whether the receiver requires all unarchived classes to conform to NSSecureCoding.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var requiresSecureCoding: Bool { get set }
```

## Parameters 

`flag`  

true if the receiver requires NSSecureCoding; false if not.

## Discussion

If you set the receiver to require secure coding, it will throw an exception if you attempt to unarchive a class which does not conform to NSSecureCoding.

The secure coding requirement for NSKeyedUnarchiver is designed to be set once at the top level and remain on. Once enabled, attempting to call `setRequiresSecureCoding:` with a value of false will throw an exception. This is to prevent classes from selectively turning secure coding off.

Note that the getter is on the superclass, NSCoder. See NSCoder for more information about secure coding.

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

class func unarchiveObject(with: Data) -> Any?

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` and stored in a given `NSData` object.

Deprecated

class func unarchiveObject(withFile: String) -> Any?

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` written to the file at a given path.

Deprecated

