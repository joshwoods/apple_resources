

- RealityKit
- AnimationHandoffType
-  default 

Type Property

# default

Provides the default behavior.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static var `default`: AnimationHandoffType { get }
```

## Discussion

If the `layerId` in the `playAnimation()` call is a non-zero value, the default behavior is a compose handoff . If the `layerId` is `0,` then the default behavior is a `snapshotAndReplace(applyToAllLayers: true)` handoff.

