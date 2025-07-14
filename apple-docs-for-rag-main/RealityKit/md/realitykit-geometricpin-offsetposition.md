

- RealityKit
- GeometricPin
-  offsetPosition 

Instance Property

# offsetPosition

Offset from the pin’s base position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var offsetPosition: SIMD3 { get set }
```

## Discussion

If a pin has a generic name, this offset is relative to the pin’s owning entity’s position. If a pin is on a skeletal joint, this offset is relative to the skeletal joint’s current position. By default this offset is the zero position vector.

