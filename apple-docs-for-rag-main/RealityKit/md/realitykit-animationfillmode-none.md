

- RealityKit
- AnimationFillMode
-  none 

Type Property

# none

An option that indicates an animation doesn’t display frame data outside of its normal duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static let none: AnimationFillMode
```

## Discussion

For example, if you rewind an animation of a hand waving for one second by setting trimStart to `-1.0`, a fillMode of `none` determines that the hand is invisible for one second before appearing and waving.

## See Also

### Choosing a fill mode

static let forwards: AnimationFillMode

An option that freezes the last frame of the animation until it stops.

static let backwards: AnimationFillMode

An option that shows the first animation frame while playback progresses to the beginning position.

static let both: AnimationFillMode

An option that displays the animation’s initial frame or final frame when playback occurs outside of the normal duration.

let rawValue: Int8

The corresponding value of the raw type.

