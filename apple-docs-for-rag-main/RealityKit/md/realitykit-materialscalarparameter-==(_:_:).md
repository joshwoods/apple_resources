

- RealityKit
- MaterialScalarParameter
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two scalar parameters are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static func == (lhs: MaterialScalarParameter, rhs: MaterialScalarParameter) -> Bool
```

## Parameters 

`lhs`  

The first scalar parameter to compare.

`rhs`  

The second scalar parameter to compare.

## Return Value

A Boolean value set to `true` if the two scalar parameters are equal.

## See Also

### Comparing material scalar parameters

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the scalar parameter by feeding them into the given hash function.

var hashValue: Int

The hash value.

