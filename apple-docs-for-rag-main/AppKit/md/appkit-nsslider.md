

- AppKit
-  NSSlider 

Class

# NSSlider

A display of a bar representing a continuous range of numerical values and a knob representing the currently selected value.

macOS

``` source
@MainActor
class NSSlider
```

## Overview

A slider is a UI element that displays a range of values in the app. Sliders can be vertical or horizontal bars or circular dials. An indicator, or knob, notes the current setting. The user can move the knob in the slider’s bar—or rotate the knob in a circular slider—to change the setting.

The `NSSlider` class uses the NSSliderCell class to implement its user interface.

## Topics

### Creating Sliders

convenience init(target: Any?, action: Selector?)

Creates a continuous horizontal slider whose values range from `0.0` to `1.0`.

convenience init(value: Double, minValue: Double, maxValue: Double, target: Any?, action: Selector?)

Creates a continuous horizontal slider that represents values over the specified range.

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

var trackFillColor: NSColor?

The color of the filled portion of the slider track, in appearances that support it.

### Asking About the Value Limits

var maxValue: Double

The maximum value the slider can send to its target.

var minValue: Double

The minimum value the slider can send to its target.

### Handling Mouse-Down Events

func acceptsFirstMouse(for: NSEvent?) -> Bool

Returns a Boolean value indicating whether a mouse-down event both activates the window and starts dragging the slider’s knob.

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value that indicates whether the slider fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the given point.

var numberOfTickMarks: Int

The number of tick marks associated with the slider.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the given index.

var tickMarkPosition: NSSlider.TickMarkPosition

Determines where the slider’s tick marks are displayed.

enum TickMarkPosition

The position where a linear slider’s tick marks appear (above, below, leading, or trailing).

func tickMarkValue(at: Int) -> Double

Returns the slider’s value represented by the tick mark at the specified index.

## Relationships

### Inherits From

- NSControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAccessibilitySlider
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

