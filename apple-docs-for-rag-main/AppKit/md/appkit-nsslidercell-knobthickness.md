

- AppKit
- NSSliderCell
-  knobThickness 

Instance Property

# knobThickness

The thickness of the slider knob, in pixels.

macOS

``` source
@MainActor
var knobThickness: CGFloat { get }
```

## Discussion

The thickness is defined to be the extent of the knob along the long dimension of the bar. In a vertical slider, a knob’s thickness is its height; in a horizontal slider, its thickness is its width.

## See Also

### Managing Cell Appearance

var isVertical: Bool

An integer indicating the orientation (vertical or horizontal) of the slider.

