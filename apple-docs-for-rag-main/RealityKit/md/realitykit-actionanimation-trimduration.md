

- RealityKit
- ActionAnimation
-  trimDuration 

Instance Property

# trimDuration

An optional duration that overrides the calculated duration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var trimDuration: TimeInterval? { get set }
```

## Discussion

The framework calculates `AnimationAction/duration`, but you can set this property to override it. This property is `nil` by default, which indicates that the animation stops after one play that spans `AnimationAction/duration`.

If you set a value for this property and both `AnimationAction/trimStart` and `AnimationAction/trimEnd` are `nil`, the animation observes this property as an edited duration.

A value greater than `AnimationAction/duration` causes the animation to repeat, applying the characteristics defined by `AnimationAction/repeatMode`. Assign this property greatestFiniteMagnitude to repeat indefinitely.

