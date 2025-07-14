

- RealityKit
- BoundingBox
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values `a` and `b`, `a != b` implies that `a == b` is `false`.

This is the default implementation of the not-equal-to operator (`!=`) for any type that conforms to `Equatable`.

## See Also

### Comparing bounding boxes

static func == (BoundingBox, BoundingBox) -> Bool

Indicates whether two bounding boxes are equal.

func hash(into: inout Hasher)

Hashes the essential components of the bounding box by feeding them into the given hash function.

var hashValue: Int

The hash value.

