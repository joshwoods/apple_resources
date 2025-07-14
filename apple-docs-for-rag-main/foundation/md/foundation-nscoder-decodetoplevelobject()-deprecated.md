

- Foundation
- NSCoder
-  decodeTopLevelObject() Deprecated

Instance Method

# decodeTopLevelObject()

Decodes a previously-encoded object.

iOS 9.0–18.4DeprecatediPadOS 9.0–18.4DeprecatedMac Catalyst 9.0–18.4DeprecatedmacOS 10.11–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
@nonobjc
func decodeTopLevelObject() throws -> Any?
```

Deprecated

Use decodeTopLevelObject(of:forKey:) instead

## Return Value

The decoded object, or `nil` if decoding fails.

## See Also

### Decoding Top-Level Objects

func decodeObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) -> DecodedObjectType?

Decode an object as an expected type, failing if the archived type doesn’t match.

func decodeObject(of: [AnyClass]?, forKey: String) -> Any?

Decode an object as one of several expected types, failing if the archived type doesn’t match any of the types.

func decodeTopLevelObject(forKey: String) throws -> Any?

Decodes the previously-encoded object associated by a key.

func decodeTopLevelObject&lt;DecodedObjectType>(of: DecodedObjectType.Type, forKey: String) throws -> DecodedObjectType?

Decode an object as one of several expected types, failing if the archived type does not match.

func decodeTopLevelObject(of: [AnyClass]?, forKey: String) throws -> Any?

Decode an object as one of several expected types, failing if the archived type does not match.

