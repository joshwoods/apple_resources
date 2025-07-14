

- RealityKit
- EntityGeometricPins
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var underestimatedCount: Int { get }
```

## Discussion

The default implementation returns 0. If you provide your own implementation, make sure to compute the value nondestructively.

Complexity

O(1), except if the sequence also conforms to `Collection`. In this case, see the documentation of `Collection.underestimatedCount`.

