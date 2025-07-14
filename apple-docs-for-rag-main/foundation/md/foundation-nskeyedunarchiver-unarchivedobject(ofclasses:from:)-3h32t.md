

- Foundation
- NSKeyedUnarchiver
-  unarchivedObject(ofClasses:from:) 

Type Method

# unarchivedObject(ofClasses:from:)

Decodes a previously-archived object graph, returning the root object as one of the specified classes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@nonobjc
static func unarchivedObject(
    ofClasses classes: [AnyClass],
    from data: Data
) throws -> Any?
```

## Parameters 

`classes`  

A set of classes, at least one of which the root object should conform to.

`data`  

An object graph previously encoded by NSKeyedArchiver.

## Return Value

The decoded root of the object graph, as an instance of one of the specified classes, or `nil` if an error occurred.

## Discussion

This method produces an error if `data` does not contain valid keyed data.

Important

Make sure you have adopted NSSecureCoding in the types you decode. If any call to a `decode`-prefixed method fails, the default decodingFailurePolicy sets the error rather than throwing an exception. In this case, the current and all subsequent decode calls return `0` or `nil`.

## See Also

### Unarchiving Data

class func unarchiveTopLevelObjectWithData(Data) throws -> Any?

Decodes a previously-archived object graph, and returns the root object.

static func unarchivedObject&lt;DecodedObjectType>(ofClass: DecodedObjectType.Type, from: Data) throws -> DecodedObjectType?

Decodes a previously-archived object graph, and returns the root object as the specified type.

class func unarchivedObject(ofClasses: Set&lt;AnyHashable>, from: Data) throws -> Any

Decodes a previously-archived object graph, returning the root object as one of the specified classes.

var requiresSecureCoding: Bool

Indicates whether the receiver requires all unarchived classes to conform to NSSecureCoding.

class func unarchiveObject(with: Data) -> Any?

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` and stored in a given `NSData` object.

Deprecated

class func unarchiveObject(withFile: String) -> Any?

Decodes and returns the object graph previously encoded by `NSKeyedArchiver` written to the file at a given path.

Deprecated

