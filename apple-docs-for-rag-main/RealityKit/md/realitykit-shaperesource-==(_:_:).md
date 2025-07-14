

- RealityKit
- ShapeResource
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two shapes are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func == (lhs: ShapeResource, rhs: ShapeResource) -> Bool
```

## Parameters 

`lhs`  

The first shape to compare.

`rhs`  

The second shape to compare.

## Return Value

A Boolean value set to `true` if the two shapes are equal.

## See Also

### Comparing shapes

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the shape by feeding them into the given hash function.

var hashValue: Int

The hash value.

