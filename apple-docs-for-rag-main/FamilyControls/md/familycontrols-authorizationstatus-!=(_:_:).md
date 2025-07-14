

- FamilyControls
- AuthorizationStatus
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

FamilyControlsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

The first authorization status to compare.

`rhs`  

The second authorization status to compare.

## Return Value

A Boolean value that’s set to `true` if the two authorization statuses aren’t equal.

## See Also

### Comparing Status Instances

var hashValue: Int

The hashed value of the authorization status.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

