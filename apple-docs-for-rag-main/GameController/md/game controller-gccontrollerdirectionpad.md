

- Game Controller
-  GCControllerDirectionPad 

Class

# GCControllerDirectionPad

A control element associated with a directional pad or a thumbstick.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class GCControllerDirectionPad
```

## Overview

You get the input values for this element from its subelements. You can use either the xAxis and yAxis properties to get coordinates, or the up, down, left, and right buttons that simulate directional pad buttons.

## Topics

### Accessing values using the axes

var xAxis: GCControllerAxisInput

The x-axis element of the directional pad.

var yAxis: GCControllerAxisInput

The y-axis element of the directional pad.

### Accessing values using directional buttons

var right: GCControllerButtonInput

The button element that changes the positive x-axis.

var left: GCControllerButtonInput

The button element that changes the negative x-axis.

var up: GCControllerButtonInput

The button element that changes the positive y-axis.

var down: GCControllerButtonInput

The button element used for the negative y-axis direction.

### Getting change information

var valueChangedHandler: GCControllerDirectionPadValueChangedHandler?

The block that the directional pad calls when the user changes its values.

typealias GCControllerDirectionPadValueChangedHandler

The signature for the block that executes when either axis changes values.

### Setting snapshot values

func setValueForXAxis(Float, yAxis: Float)

Sets the input values of a snapshot of a directional pad.

## Relationships

### Inherits From

- GCControllerElement

### Inherited By

- GCDeviceCursor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accessing controller elements

class GCControllerElement

An input for a physical control, such as a button or thumbstick.

class GCControllerAxisInput

A control element that tracks movement along an axis.

class GCControllerButtonInput

A control element that represents a button touch or press.

class GCControllerTouchpad

A control element that represents a touch event on a touchpad.

class GCDeviceCursor

A control element for the cursor used as a directional pad.

class GCDualSenseAdaptiveTrigger

A class that encapsulates the features of a DualSense adaptive trigger.

