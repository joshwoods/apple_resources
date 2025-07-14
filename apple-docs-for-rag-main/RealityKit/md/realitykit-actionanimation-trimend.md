

- RealityKit
- ActionAnimation
-  trimEnd 

Instance Property

# trimEnd

The optional time, in seconds, at which the animation stops.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var trimEnd: TimeInterval? { get set }
```

## Discussion

This property is `nil` by default, which plays the animation until `time` = duration. If you set a value, the animation edits the duration according to the specified ending time.

