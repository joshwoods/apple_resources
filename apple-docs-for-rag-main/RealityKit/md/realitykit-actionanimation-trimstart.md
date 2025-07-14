

- RealityKit
- ActionAnimation
-  trimStart 

Instance Property

# trimStart

The optional time, in seconds, at which the animation plays.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var trimStart: TimeInterval? { get set }
```

## Discussion

This property is `nil` by default, which plays the animation with `time` = `0`. If you set a value, the animation edits the duration according to the specified beginning time.

If you set a negative value for this property, the duration increases and the additional animation data fills in based on the fillMode you choose.

