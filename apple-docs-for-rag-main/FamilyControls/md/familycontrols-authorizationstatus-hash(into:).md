

- FamilyControls
- AuthorizationStatus
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the authorization status by feeding them into the given hash function.

FamilyControlsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func hash(into hasher: inout Hasher)
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## Parameters 

`hasher`  

The hash function to use when combining the components of the authorization status.

## See Also

### Comparing Status Instances

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

var hashValue: Int

The hashed value of the authorization status.

