

- Game Controller
-  GCControllerButtonInput 

Class

# GCControllerButtonInput

A control element that represents a button touch or press.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class GCControllerButtonInput
```

## Overview

A `GCControllerButtonInput` object represents a button on a controller that can report either analog or digital values.

## Topics

### Accessing input values

var isTouched: Bool

A Boolean value that indicates whether the user is touching the button.

var isPressed: Bool

A Boolean value that indicates whether the user is pressing the button.

var value: Float

The level of pressure the user is applying to the button.

### Getting change information

var touchedChangedHandler: GCControllerButtonTouchedChangedHandler?

The block that the element calls when the user touches the button.

typealias GCControllerButtonTouchedChangedHandler

The signature for the block that executes when the user touches the button if the controller supports that feature.

var pressedChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user presses or releases the button.

var valueChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user changes the level of pressure on the button.

typealias GCControllerButtonValueChangedHandler

The signature for the block that executes when a button’s state changes.

### Setting snapshot values

func setValue(Float)

Sets the pressure value of a snapshot of a button.

## Relationships

### Inherits From

- GCControllerElement

### Inherited By

- GCDualSenseAdaptiveTrigger

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

class GCControllerTouchpad

A control element that represents a touch event on a touchpad.

class GCControllerDirectionPad

A control element associated with a directional pad or a thumbstick.

class GCDeviceCursor

A control element for the cursor used as a directional pad.

class GCDualSenseAdaptiveTrigger

A class that encapsulates the features of a DualSense adaptive trigger.

