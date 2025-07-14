

- Foundation
- NSCoder
-  decodeObject(of:forKey:) 

Instance Method

# decodeObject(of:forKey:)

Decode an object as an expected type, failing if the archived type doesn’t match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeObject(
    of cls: DecodedObjectType.Type,
    forKey key: String
) -> DecodedObjectType? where DecodedObjectType : NSObject, DecodedObjectType : NSCoding
```

## Parameters 

`cls`  

The expected class of the object being decoded.

`key`  

The key indicating the member to decode.

## Return Value

The decoded object, or `nil` if decoding fails.

## Discussion

If the coder responds true to requiresSecureCoding, then the coder calls failWithError(_:) in either of the following cases:

- The class indicated by `cls` doesn’t implement NSSecureCoding.

- The unarchived class doesn’t match `cls`, nor do any of its superclasses.

If the coder doesn’t require secure coding, it ignores the `cls` parameter and does not check the decoded object.

## See Also

### Decoding Top-Level Objects

func decodeObject(of: [AnyClass]?, forKey: String) -> Any?

Decode an object as one of several expected types, failing if the archived type doesn’t match any of the types.

func decodeTopLevelObject() throws -> Any?

Decodes a previously-encoded object.

Deprecated

func decodeTopLevelObject(forKey: String) throws -> Any?

Decodes the previously-encoded object associated by a key.

func decodeTopLevelObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) throws -> DecodedObjectType?

Decode an object as one of several expected types, failing if the archived type does not match.

func decodeTopLevelObject(of: [AnyClass]?, forKey: String) throws -> Any?

Decode an object as one of several expected types, failing if the archived type does not match.

