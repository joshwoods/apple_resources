

- AppKit
- NSSlider
-  knobThickness 

Instance Property

# knobThickness

The knob’s thickness, in pixels.

macOS

``` source
@MainActor
var knobThickness: CGFloat { get }
```

## Discussion

The thickness is defined to be the extent of the knob along the long dimension of the bar. In a vertical slider, a knob’s thickness is its height; in a horizontal slider, a knob’s thickness is its width.

## See Also

### Managing the Slider’s Appearance

var sliderType: NSSlider.SliderType

The type of the slider, such as vertical or circular.

enum SliderType

The types of sliders, used by sliderType.

var altIncrementValue: Double

The amount by which the slider changes its value when the user Option-drags the slider knob.

var isVertical: Bool

An integer indicating the orientation (horizontal or vertical) of the slider.

var trackFillColor: NSColor?

The color of the filled portion of the slider track, in appearances that support it.

