

- Game Controller
-  GCDualSenseAdaptiveTrigger 

Class

# GCDualSenseAdaptiveTrigger

A class that encapsulates the features of a DualSense adaptive trigger.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
class GCDualSenseAdaptiveTrigger
```

## Overview

A `GCDualSenseAdaptiveTrigger` object allows you to specify a dynamic resistance force that the DualSense controller applies when the user pulls the trigger. For example, set the resistance to give the user the feeling of pulling back on a bow string, firing a weapon, or pulling a lever.

## Topics

### Getting the mode

var mode: GCDualSenseAdaptiveTrigger.Mode

The current configuration of the adaptive trigger.

enum Mode

The possible modes of an adaptive trigger.

func setModeOff()

Sets the mode to off and stops any trigger effect.

### Configuring the trigger

func setModeFeedbackWithStartPosition(Float, resistiveStrength: Float)

Sets the mode to provide feedback when the user depresses the trigger at the start position or at a greater value.

struct PositionalResistiveStrengths

The resistive strengths for multiple positions on a trigger.

func setModeFeedback(resistiveStrengths: GCDualSenseAdaptiveTrigger.PositionalResistiveStrengths)

Sets the mode to provide feedback with the specified strengths for each possible trigger position.

func setModeWeaponWithStartPosition(Float, endPosition: Float, resistiveStrength: Float)

Sets the mode to provide feedback when the user depresses the trigger between the start and the end positions.

func setModeVibrationWithStartPosition(Float, amplitude: Float, frequency: Float)

Sets the mode to vibrate when the user depresses the trigger at the start position or at a greater value.

func setModeVibration(amplitudes: GCDualSenseAdaptiveTrigger.PositionalAmplitudes, frequency: Float)

Sets the mode to vibrate with the specified amplitudes for each possible trigger position.

struct PositionalAmplitudes

The amplitudes for multiple positions on a trigger.

func setModeSlopeFeedback(startPosition: Float, endPosition: Float, startStrength: Float, endStrength: Float)

Sets the mode to provide feedback when the user tilts the trigger between the start and the end positions.

### Getting the arm position

var armPosition: Float

The position of the trigger’s arm.

class var discretePositionCount: Int

The number of discrete control positions that the DualSense adaptive triggers support.

### Checking the status

var status: GCDualSenseAdaptiveTrigger.Status

The current status of the adaptive trigger and whether it’s applying effects.

enum Status

The possible states of an adaptive trigger.

## Relationships

### Inherits From

- GCControllerButtonInput

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

class GCControllerDirectionPad

A control element associated with a directional pad or a thumbstick.

class GCDeviceCursor

A control element for the cursor used as a directional pad.

