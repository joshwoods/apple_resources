

- Objective-C Runtime
- NSObject
-  handleQuery(withUnboundKey:) Deprecated

Instance Method

# handleQuery(withUnboundKey:)

Invoked by value(forKey:) when it finds no property corresponding to `key`.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func handleQuery(withUnboundKey key: String) -> Any?
```

Deprecated

Use value(forUndefinedKey:) instead.

## See Also

### Deprecated Methods

class func useStoredAccessor() -> Bool

Returns `true` if the stored value methods storedValue(forKey:) and takeStoredValue(_:forKey:) should use private accessor methods in preference to public accessors.

Deprecated

func handleTakeValue(Any?, forUnboundKey: String)

Invoked by takeValue(_:forKey:) when it finds no property binding for `key`.

Deprecated

func storedValue(forKey: String) -> Any?

Returns the property identified by a given key.

Deprecated

func takeStoredValue(Any?, forKey: String)

Sets the value of the property identified by a given key.

Deprecated

func takeValues(from: [AnyHashable : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties

Deprecated

func takeValue(Any?, forKeyPath: String)

Sets the value for the property identified by `keyPath` to `value`.

Deprecated

func takeValue(Any?, forKey: String)

Sets the value for the property identified by `key` to `value`.

Deprecated

func unableToSetNil(forKey: String)

Invoked if `key` is represented by a scalar attribute.

Deprecated

func values(forKeys: [Any]) -> [AnyHashable : Any]

Returns a dictionary containing as keys the property names in `keys`, with corresponding values being the corresponding property values.

Deprecated

