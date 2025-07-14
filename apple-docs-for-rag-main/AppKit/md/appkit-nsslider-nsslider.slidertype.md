

- AppKit
- NSSlider
-  NSSlider.SliderType 

Enumeration

# NSSlider.SliderType

The types of sliders, used by sliderType.

macOS

``` source
enum SliderType
```

## Topics

### Enumeration Cases

case circular

A dial representing an angular range.

case linear

A bar representing a range, and a knob indicating the currently selected value.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the Slider’s Appearance

var sliderType: NSSlider.SliderType

The type of the slider, such as vertical or circular.

var altIncrementValue: Double

The amount by which the slider changes its value when the user Option-drags the slider knob.

var knobThickness: CGFloat

The knob’s thickness, in pixels.

var isVertical: Bool

An integer indicating the orientation (horizontal or vertical) of the slider.

var trackFillColor: NSColor?

The color of the filled portion of the slider track, in appearances that support it.

