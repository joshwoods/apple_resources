

- Metal
- MTLTriangleTessellationFactorsHalf
-  edgeTessellationFactor 

Instance Property

# edgeTessellationFactor

The edge tessellation factors, with each index value providing the tessellation factor for a particular edge.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var edgeTessellationFactor: (UInt16, UInt16, UInt16)
```

## Discussion

- The value in index 0 provides the tessellation factor for the upper-left edge of the patch.

- The value in index 1 provides the tessellation factor for the bottom edge of the patch.

- The value in index 2 provides the tessellation factor for the upper-right edge of the patch.

## See Also

### Instance Properties

var insideTessellationFactor: UInt16

The inside tessellation factor.

