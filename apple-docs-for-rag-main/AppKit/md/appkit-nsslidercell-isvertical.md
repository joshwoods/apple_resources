

- AppKit
- NSSliderCell
-  isVertical 

Instance Property

# isVertical

An integer indicating the orientation (vertical or horizontal) of the slider.

macOS 10.11+

``` source
@MainActor
var isVertical: Bool { get set }
```

``` source
var vertical: Bool { get set }
```

## Discussion

The value of this property is 1 if the slider is vertical, 0 if it’s horizontal, and –1 if the orientation can’t be determined (for example, if the slider hasn’t been displayed yet). A slider is defined as vertical if its height is greater than its width.

## See Also

### Managing Cell Appearance

var knobThickness: CGFloat

The thickness of the slider knob, in pixels.

