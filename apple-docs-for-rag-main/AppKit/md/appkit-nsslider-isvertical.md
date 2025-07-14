

- AppKit
- NSSlider
-  isVertical 

Instance Property

# isVertical

An integer indicating the orientation (horizontal or vertical) of the slider.

macOS 10.12+

``` source
@MainActor
var isVertical: Bool { get set }
```

``` source
var vertical: Bool { get set }
```

## Discussion

The value of this property is `1` if the slider is vertical, `0` if it’s horizontal, and `-1` if the orientation is unknown (for example, if the slider hasn’t been displayed yet). A slider is defined as vertical if its height is greater than its width.

## See Also

### Managing the Slider’s Appearance

var sliderType: NSSlider.SliderType

The type of the slider, such as vertical or circular.

enum SliderType

The types of sliders, used by sliderType.

var altIncrementValue: Double

The amount by which the slider changes its value when the user Option-drags the slider knob.

var knobThickness: CGFloat

The knob’s thickness, in pixels.

var trackFillColor: NSColor?

The color of the filled portion of the slider track, in appearances that support it.

