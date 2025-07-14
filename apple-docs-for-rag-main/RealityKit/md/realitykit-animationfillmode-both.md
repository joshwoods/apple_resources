

- RealityKit
- AnimationFillMode
-  both 

Type Property

# both

An option that displays the animation’s initial frame or final frame when playback occurs outside of the normal duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static let both: AnimationFillMode
```

## Discussion

For example, if you extend a hand-waving animation’s duration by one second in both directions by setting trimStart to `-1.0`, and trimEnd to duration + `1.0`, a fillMode of `both` determines that the hand holds its initial appearance for one second before continuing to wave. Then, the animation freezes on its final hand-waving frame for one second before disappearing.

## See Also

### Choosing a fill mode

static let none: AnimationFillMode

An option that indicates an animation doesn’t display frame data outside of its normal duration.

static let forwards: AnimationFillMode

An option that freezes the last frame of the animation until it stops.

static let backwards: AnimationFillMode

An option that shows the first animation frame while playback progresses to the beginning position.

let rawValue: Int8

The corresponding value of the raw type.

