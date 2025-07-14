

- Metal
-  MTLPackedFloat4x3 

Type Alias

# MTLPackedFloat4x3

A structure that contains the top three rows of a 4x4 matrix of 32-bit floating-point values, in column-major order.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLPackedFloat4x3 = _MTLPackedFloat4x3
```

## Discussion

Metal uses the values `[0,0,0,1]` as the bottom row of the `4x4` matrix.

## See Also

### Supporting Types

typealias MTLAxisAlignedBoundingBox

The bounds for an axis-aligned bounding box.

typealias MTLPackedFloat3

A structure that contains three 32-bit floating-point values with no additional padding.

func MTLPackedFloat3Make(Float, Float, Float) -> MTLPackedFloat3

Returns a new packed vector with three floating-point values.

