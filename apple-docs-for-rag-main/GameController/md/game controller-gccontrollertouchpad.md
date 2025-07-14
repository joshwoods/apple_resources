

- Game Controller
-  GCControllerTouchpad 

Class

# GCControllerTouchpad

A control element that represents a touch event on a touchpad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class GCControllerTouchpad
```

## Overview

A `GCControllerTouchpad` object provides the state of the touches and presses on a touchpad. This is a compound element with button and directional pad subelements.

## Topics

### Getting the subelements

var touchSurface: GCControllerDirectionPad

The element that represents the state of the user’s touch on the surface of the touchpad.

var button: GCControllerButtonInput

The element that represents the button component on the touchpad.

### Accessing the input values

var touchState: GCControllerTouchpad.TouchState

The state of the user’s touch on the surface of the touchpad.

enum TouchState

The possible states of the user’s touch.

var reportsAbsoluteTouchSurfaceValues: Bool

A Boolean value that determines whether the touch values are absolute or relative.

### Getting change information

var touchDown: GCControllerTouchpadHandler?

The block that the element calls when the user begins touching the touchpad.

var touchMoved: GCControllerTouchpadHandler?

The block that the element calls when the user continues touching the touchpad, not when the user begins or ends touching the touchpad.

var touchUp: GCControllerTouchpadHandler?

The block that the element calls when the user finishes touching the touchpad.

typealias GCControllerTouchpadHandler

The signature for the block that executes when the user interacts with the touchpad.

### Setting snapshot values

func setValueForXAxis(Float, yAxis: Float, touchDown: Bool, buttonValue: Float)

Sets the input values of a snapshot of a touchpad.

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

class GCControllerAxisInput

A control element that tracks movement along an axis.

class GCControllerButtonInput

A control element that represents a button touch or press.

class GCControllerDirectionPad

A control element associated with a directional pad or a thumbstick.

class GCDeviceCursor

A control element for the cursor used as a directional pad.

class GCDualSenseAdaptiveTrigger

A class that encapsulates the features of a DualSense adaptive trigger.

