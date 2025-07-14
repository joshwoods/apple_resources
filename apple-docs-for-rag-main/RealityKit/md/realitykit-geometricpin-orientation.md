

- RealityKit
- GeometricPin
-  orientation 

Instance Property

# orientation

Calculates and returns the current orientation of the pin relative to the pin’s owning entity, adjusted by the optional offset orientation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
var orientation: simd_quatf? { get }
```

## Discussion

If the pin is on a skeletal joint but there is no skeletal joint matching the given skeletal joint name, this property returns `nil`.

