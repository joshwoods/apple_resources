

- Game Controller
-  GCControllerAxisInput 

Class

# GCControllerAxisInput

A control element that tracks movement along an axis.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class GCControllerAxisInput
```

## Overview

A `GCControllerAxisInput` object represents the value of a physical controller’s axis. For example, a GCControllerDirectionPad has x-axis and y-axis subelements.

## Topics

### Accessing the input values

var value: Float

The current value of the axis.

func setValue(Float)

Sets the normalized value of the axis.

### Getting change information

var valueChangedHandler: GCControllerAxisValueChangedHandler?

The block that the element calls when the user changes the axis value.

typealias GCControllerAxisValueChangedHandler

The signature for the block that executes when the user changes the axis value.

## Relationships

### Inherits From

- GCControllerElement

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

class GCControllerButtonInput

A control element that represents a button touch or press.

class GCControllerTouchpad

A control element that represents a touch event on a touchpad.

class GCControllerDirectionPad

A control element associated with a directional pad or a thumbstick.

class GCDeviceCursor

A control element for the cursor used as a directional pad.

class GCDualSenseAdaptiveTrigger

A class that encapsulates the features of a DualSense adaptive trigger.

