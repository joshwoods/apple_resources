

- RealityKit
- MaterialColorParameter
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two color parameters are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static func == (lhs: MaterialColorParameter, rhs: MaterialColorParameter) -> Bool
```

## Parameters 

`lhs`  

The first color parameter to compare.

`rhs`  

The second color parameter to compare.

## Return Value

A Boolean value set to `true` if the two color parameters are equal.

## See Also

### Comparing material color parameters

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the color parameter by feeding them into the given hash function.

var hashValue: Int

The hash value.

