

- RealityKit
- AnimationFillMode
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
let rawValue: Int8
```

## Discussion

A new instance initialized with `rawValue` will be equivalent to this instance. For example:

```
enum PaperSize: String {
    case A4, A5, Letter, Legal
}

let selectedSize = PaperSize.Letter
print(selectedSize.rawValue)
// Prints "Letter"

print(selectedSize == PaperSize(rawValue: selectedSize.rawValue)!)
// Prints "true"
```

## See Also

### Choosing a fill mode

static let none: AnimationFillMode

An option that indicates an animation doesn’t display frame data outside of its normal duration.

static let forwards: AnimationFillMode

An option that freezes the last frame of the animation until it stops.

static let backwards: AnimationFillMode

An option that shows the first animation frame while playback progresses to the beginning position.

static let both: AnimationFillMode

An option that displays the animation’s initial frame or final frame when playback occurs outside of the normal duration.

