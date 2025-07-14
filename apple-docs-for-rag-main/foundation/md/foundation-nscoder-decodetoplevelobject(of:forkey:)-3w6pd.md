

- Foundation
- NSCoder
-  decodeTopLevelObject(of:forKey:) 

Instance Method

# decodeTopLevelObject(of:forKey:)

Decode an object as one of several expected types, failing if the archived type does not match.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeTopLevelObject(
    of cls: DecodedObjectType.Type,
    forKey key: String
) throws -> DecodedObjectType? where DecodedObjectType : NSObject, DecodedObjectType : NSCoding
```

## Parameters 

`cls`  

The expected class of the object being decoded.

`key`  

The key indicating the member to decode.

## Return Value

The decoded object, or `nil` if decoding fails.

## Discussion

If the coder responds true to requiresSecureCoding, then the coder calls failWithError(_:) in either the following cases:

- The class indicated by `cls` does not implement NSSecureCoding.

- The unarchived class does not match `cls`, nor do any of its superclasses.

If the coder does not require secure coding, it ignores the `cls` parameter and does not check the decoded object.

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

func decodeTopLevelObject(of: [AnyClass]?, forKey: String) throws -> Any?

Decode an object as one of several expected types, failing if the archived type does not match.

