

- RealityKit
- PlayAnimationAction
-  separateAnimatedValue 

Instance Property

# separateAnimatedValue

When set to false, this value indicates that the animation will write directly to the entity’s base value. When set to true, this value indicates that the animation will write to an interim value for the duration of the animation. If this value is set to true then when the animation completes, the entity’s value will be reset to the base value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var separateAnimatedValue: Bool
```

