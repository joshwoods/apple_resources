

- Game Controller
- GCDualSenseAdaptiveTrigger
-  setModeFeedback(resistiveStrengths:) 

Instance Method

# setModeFeedback(resistiveStrengths:)

Sets the mode to provide feedback with the specified strengths for each possible trigger position.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func setModeFeedback(resistiveStrengths positionalResistiveStrengths: GCDualSenseAdaptiveTrigger.PositionalResistiveStrengths)
```

## Parameters 

`positionalResistiveStrengths`  

The resistance values for each possible trigger position.

## See Also

### Configuring the trigger

func setModeFeedbackWithStartPosition(Float, resistiveStrength: Float)

Sets the mode to provide feedback when the user depresses the trigger at the start position or at a greater value.

struct PositionalResistiveStrengths

The resistive strengths for multiple positions on a trigger.

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

