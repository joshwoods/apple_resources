

- RealityKit
- BoundingBox
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two bounding boxes are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static func == (lhs: BoundingBox, rhs: BoundingBox) -> Bool
```

## Parameters 

`lhs`  

The first box to compare.

`rhs`  

The second box to compare.

## Return Value

A Boolean value set to `true` if the two boxes are equal.

## See Also

### Comparing bounding boxes

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the bounding box by feeding them into the given hash function.

var hashValue: Int

The hash value.

