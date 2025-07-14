

- RealityKit
- ForceEffectParameters
-  positions 

Instance Property

# positions

The positions of all rigid bodies under the influence of the effect, or nil if positional information was not requested.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let positions: UnsafeForceEffectBuffer>?
```

## Discussion

The position is located at each body’s center of mass, relative to the origin of the effect.

