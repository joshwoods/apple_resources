

- AppKit
- NSSlider
-  sliderType 

Instance Property

# sliderType

The type of the slider, such as vertical or circular.

macOS 10.10+

``` source
@MainActor
var sliderType: NSSlider.SliderType { get set }
```

## Discussion

See NSSlider.SliderType for possible values.

## See Also

### Managing the Slider’s Appearance

enum SliderType

The types of sliders, used by sliderType.

var altIncrementValue: Double

The amount by which the slider changes its value when the user Option-drags the slider knob.

var knobThickness: CGFloat

The knob’s thickness, in pixels.

var isVertical: Bool

An integer indicating the orientation (horizontal or vertical) of the slider.

var trackFillColor: NSColor?

The color of the filled portion of the slider track, in appearances that support it.

