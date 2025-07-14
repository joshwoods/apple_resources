

- RealityKit
- ActionAnimation
-  duration 

Instance Property

# duration

The elapsed time for one complete rotation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var duration: TimeInterval { get }
```

## Discussion

The framework sets a value for this property depending on the underlying animation data and the specified `AnimationAction/speed`.

You can override the default duration by defining `AnimationAction/trimStart`, `AnimationAction/trimEnd`, or `AnimationAction/trimDuration`.

