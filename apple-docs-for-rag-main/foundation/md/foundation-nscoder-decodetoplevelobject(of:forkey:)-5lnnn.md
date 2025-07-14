

- Foundation
- NSCoder
-  decodeTopLevelObject(of:forKey:) 

Instance Method

# decodeTopLevelObject(of:forKey:)

Decode an object as one of several expected types, failing if the archived type does not match.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@nonobjc
func decodeTopLevelObject(
    of classes: [AnyClass]?,
    forKey key: String
) throws -> Any?
```

## Parameters 

`classes`  

An array of expected classes that the object being decoded should match at least one of.

`key`  

The key indicating the member to decode.

## Return Value

The decoded object, or `nil` if decoding fails.

## Discussion

This method is equivalent to decodeObject(of:forKey:), but allows you to specify a set of classes that the decoded object can match. If requiresSecureCoding is `true`, the decoded object’s class must be a member of the classes parameter, or a sublcass of a member.

## See Also

### Decoding Top-Level Objects

func decodeObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) -> DecodedObjectType?

Decode an object as an expected type, failing if the archived type doesn’t match.

func decodeObject(of: [AnyClass]?, forKey: String) -> Any?

Decode an object as one of several expected types, failing if the archived type doesn’t match any of the types.

func decodeTopLevelObject() throws -> Any?

Decodes a previously-encoded object.

Deprecated

func decodeTopLevelObject(forKey: String) throws -> Any?

Decodes the previously-encoded object associated by a key.

func decodeTopLevelObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) throws -> DecodedObjectType?

Decode an object as one of several expected types, failing if the archived type does not match.

