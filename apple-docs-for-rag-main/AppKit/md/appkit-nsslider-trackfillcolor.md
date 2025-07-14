

- AppKit
- NSSlider
-  trackFillColor 

Instance Property

# trackFillColor

The color of the filled portion of the slider track, in appearances that support it.

macOS 10.12.2+

``` source
@NSCopying @MainActor
var trackFillColor: NSColor? { get set }
```

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

var isVertical: Bool

An integer indicating the orientation (horizontal or vertical) of the slider.

