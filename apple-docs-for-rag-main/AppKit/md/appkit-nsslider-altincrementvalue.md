

- AppKit
- NSSlider
-  altIncrementValue 

Instance Property

# altIncrementValue

The amount by which the slider changes its value when the user Option-drags the slider knob.

macOS

``` source
@MainActor
var altIncrementValue: Double { get set }
```

## Discussion

By default, the value of this property is `-1.0`, and the slider behaves no differently with the Option key down than with it up. The value of this property must fit the range of values the slider can represent—for example, if the slider has a minimum value of `5` and a maximum value of `10`, the value should be between `0` and `5`.

## See Also

### Managing the Slider’s Appearance

var sliderType: NSSlider.SliderType

The type of the slider, such as vertical or circular.

enum SliderType

The types of sliders, used by sliderType.

var knobThickness: CGFloat

The knob’s thickness, in pixels.

var isVertical: Bool

An integer indicating the orientation (horizontal or vertical) of the slider.

var trackFillColor: NSColor?

The color of the filled portion of the slider track, in appearances that support it.

