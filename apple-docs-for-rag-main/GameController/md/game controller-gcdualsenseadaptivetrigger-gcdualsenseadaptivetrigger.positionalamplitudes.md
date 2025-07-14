

- Game Controller
- GCDualSenseAdaptiveTrigger
-  GCDualSenseAdaptiveTrigger.PositionalAmplitudes 

Structure

# GCDualSenseAdaptiveTrigger.PositionalAmplitudes

The amplitudes for multiple positions on a trigger.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
struct PositionalAmplitudes
```

## Topics

### Creating multiple amplitudes

init(values: (Float, Float, Float, Float, Float, Float, Float, Float, Float, Float))

Creates a positional amplitudes structure with the specified amplitude values.

init()

Creates an empty positional amplitudes structure.

### Accessing multiple amplitudes

var values: (Float, Float, Float, Float, Float, Float, Float, Float, Float, Float)

The amplitude values for possible trigger positions.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

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

func setModeSlopeFeedback(startPosition: Float, endPosition: Float, startStrength: Float, endStrength: Float)

Sets the mode to provide feedback when the user tilts the trigger between the start and the end positions.

