

- FamilyControls
- AuthorizationStatus
-  hashValue 

Instance Property

# hashValue

The hashed value of the authorization status.

FamilyControlsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var hashValue: Int { get }
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Comparing Status Instances

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

