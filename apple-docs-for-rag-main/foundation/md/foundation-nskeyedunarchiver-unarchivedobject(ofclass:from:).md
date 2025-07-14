

- Foundation
- NSKeyedUnarchiver
-  unarchivedObject(ofClass:from:) 

Type Method

# unarchivedObject(ofClass:from:)

Decodes a previously-archived object graph, and returns the root object as the specified type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@nonobjc
static func unarchivedObject(
    ofClass cls: DecodedObjectType.Type,
    from data: Data
) throws -> DecodedObjectType? where DecodedObjectType : NSObject, DecodedObjectType : NSCoding
```

## Parameters 

`cls`  

The expected class of the root object.

`data`  

An object graph previously encoded by NSKeyedArchiver.

## Return Value

The decoded root of the object graph, or `nil` if an error occurred.

## Discussion

This method produces an error if `data` does not contain valid keyed data.

Important

Make sure you have adopted NSSecureCoding in the types you decode. If any call to a `decode`-prefixed method fails, the default decodingFailurePolicy sets the error rather than throwing an exception. In this case, the current and all subsequent decode calls return `0` or `nil`.

## See Also

### Unarchiving Data

class func unarchiveTopLevelObjectWithData(Data) throws -> Any?

Decodes a previously-archived object graph, and returns the root object.

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

