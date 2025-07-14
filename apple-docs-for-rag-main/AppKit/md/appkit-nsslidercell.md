

- AppKit
-  NSSliderCell 

Class

# NSSliderCell

The appearance and behavior of an NSSlider object.

macOS

``` source
@MainActor
class NSSliderCell
```

## Overview

You can customize an NSSliderCell to a certain degree, using its properties. If this doesn’t give you sufficient flexibility, you can create a subclass. In that subclass, you can override any of the following methods: knobRect(flipped:), drawBar(inside:flipped:), drawKnob(_:), and prefersTrackingUntilMouseUp.

## Topics

### Managing Cell Behavior

var altIncrementValue: Double

The amount by which the slider changes its value when the user Option-drags the knob.

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value indicating whether the `NSSliderCell` continues to track the pointer until the next mouse up.

var trackRect: NSRect

The rectangle within which the cell tracks the pointer while the mouse button is down.

### Managing the Slider Type

var sliderType: NSSlider.SliderType

The slider type, either linear or circular.

### Displaying the Cell

func barRect(flipped: Bool) -> NSRect

Returns the rectangle in which the bar is drawn.

func drawTickMarks()

Draws the slider’s tick marks.

func knobRect(flipped: Bool) -> NSRect

Returns the rectangle in which the slider knob is drawn.

func drawBar(inside: NSRect, flipped: Bool)

Draws the slider’s bar—but not its bezel or knob—inside the specified rectangle.

func drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

func drawKnob(NSRect)

Draws the slider knob in the given rectangle.

### Managing Cell Appearance

var knobThickness: CGFloat

The thickness of the slider knob, in pixels.

var isVertical: Bool

An integer indicating the orientation (vertical or horizontal) of the slider.

### Managing Value Limits

var maxValue: Double

The maximum value the slider can send to its target.

var minValue: Double

The minimum value the slider can send to its target.

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value indicating whether the receiver fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the specified point.

var numberOfTickMarks: Int

The number of tick marks associated with the slider, including the tick marks assigned to the minimum and maximum values.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the specified index.

var tickMarkPosition: NSSlider.TickMarkPosition

The position of the tick marks relative to the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index.

### Constants

enum TickMarkPosition

The position where a linear slider’s tick marks appear (above, below, leading, or trailing).

enum SliderType

The types of sliders, used by sliderType.

## Relationships

### Inherits From

- NSActionCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

