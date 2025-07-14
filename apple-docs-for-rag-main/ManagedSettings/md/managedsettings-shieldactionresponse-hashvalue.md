

- ManagedSettings
- ShieldActionResponse
-  hashValue 

Instance Property

# hashValue

The hash value.

ManagedSettingsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var hashValue: Int { get }
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## Discussion

Hash values aren’t guaranteed to be equal across different executions of your program. Don’t save hash values to use during a future execution.

Important

`hashValue` is deprecated as a Hashable requirement. To conform to Hashable, implement the hash(into:) requirement instead.

## See Also

### Comparisons

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

