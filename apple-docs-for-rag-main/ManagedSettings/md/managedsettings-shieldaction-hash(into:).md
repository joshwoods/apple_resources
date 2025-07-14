

- ManagedSettings
- ShieldAction
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

ManagedSettingsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func hash(into hasher: inout Hasher)
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## Discussion

Implement this method to conform to the Hashable protocol. The components used for hashing must be the same as the components compared in your type’s `==` operator implementation. Call `hasher.combine(_:)` with each of these components.

Important

Never call `finalize()` on hasher; it may cause a compile-time error.

## See Also

### Comparisons

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

var hashValue: Int

The hash value.

