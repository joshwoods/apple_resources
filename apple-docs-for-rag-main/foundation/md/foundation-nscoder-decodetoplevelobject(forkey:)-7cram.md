

- Foundation
- NSCoder
-  decodeTopLevelObject(forKey:) 

Instance Method

# decodeTopLevelObject(forKey:)

Decodes the previously-encoded object associated by a key.

iOS 9.0–18.4DeprecatediPadOS 9.0–18.4DeprecatedMac Catalyst 9.0–18.4DeprecatedmacOS 10.11–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0DeprecatedSwift 4.0+

``` source
@nonobjc
func decodeTopLevelObject(forKey key: String) throws -> Any?
```

## Parameters 

`key`  

The key that identifies the object to decode.

## Return Value

The decoded object, or `nil` if decoding fails.

## See Also

### Decoding Top-Level Objects

func decodeObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) -> DecodedObjectType?

Decode an object as an expected type, failing if the archived type doesn’t match.

func decodeObject(of: [AnyClass]?, forKey: String) -> Any?

Decode an object as one of several expected types, failing if the archived type doesn’t match any of the types.

func decodeTopLevelObject() throws -> Any?

Decodes a previously-encoded object.

Deprecated

func decodeTopLevelObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) throws -> DecodedObjectType?

Decode an object as one of several expected types, failing if the archived type does not match.

func decodeTopLevelObject(of: [AnyClass]?, forKey: String) throws -> Any?

Decode an object as one of several expected types, failing if the archived type does not match.

