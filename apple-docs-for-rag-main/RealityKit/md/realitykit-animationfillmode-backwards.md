

- RealityKit
- AnimationFillMode
-  backwards 

Type Property

# backwards

An option that shows the first animation frame while playback progresses to the beginning position.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static let backwards: AnimationFillMode
```

## Discussion

For example, if you wind a hand-waving animation’s duration back one second by setting trimStart to `-1.0`, a fillMode of `backwards` determines that the hand holds its initial appearance for one second before waving.

## See Also

### Choosing a fill mode

static let none: AnimationFillMode

An option that indicates an animation doesn’t display frame data outside of its normal duration.

static let forwards: AnimationFillMode

An option that freezes the last frame of the animation until it stops.

static let both: AnimationFillMode

An option that displays the animation’s initial frame or final frame when playback occurs outside of the normal duration.

let rawValue: Int8

The corresponding value of the raw type.

