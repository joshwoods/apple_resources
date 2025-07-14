

- RealityKit
- ActionAnimation
-  fillMode 

Instance Property

# fillMode

An option that determines which data displays outside of the normal duration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var fillMode: AnimationFillMode { get set }
```

## Discussion

This property determines what to display when the framework samples the animation outside of the range defined by its underlying duration. The animation applies this property when:

- Playback progresses toward, but hasn’t yet reached, a nonzero offset. - A range determined by trimStart, trimEnd, or trimDuration exceeds the animation’s underlying duration.

