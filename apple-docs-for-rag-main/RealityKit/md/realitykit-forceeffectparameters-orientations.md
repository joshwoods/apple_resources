

- RealityKit
- ForceEffectParameters
-  orientations 

Instance Property

# orientations

The orientations of all rigid bodies under the influence of the effect, or nil if rotational information was not requested.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let orientations: UnsafeForceEffectBuffer?
```

## Discussion

The orientation is relative to the effect’s transform.

