

- RealityKit
- AnimationFillMode
-  forwards 

Type Property

# forwards

An option that freezes the last frame of the animation until it stops.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static let forwards: AnimationFillMode
```

## Discussion

For example, if you increase a hand-waving animation’s duration one second by setting trimEnd to duration + `1.0`, a fillMode of `forwards` determines that the hand waves and then freezes on its final animation frame for one second before disappearing.

## See Also

### Choosing a fill mode

static let none: AnimationFillMode

An option that indicates an animation doesn’t display frame data outside of its normal duration.

static let backwards: AnimationFillMode

An option that shows the first animation frame while playback progresses to the beginning position.

static let both: AnimationFillMode

An option that displays the animation’s initial frame or final frame when playback occurs outside of the normal duration.

let rawValue: Int8

The corresponding value of the raw type.

