

- Game Controller
- GCDualSenseAdaptiveTrigger
-  setModeVibrationWithStartPosition(\_:amplitude:frequency:) 

Instance Method

# setModeVibrationWithStartPosition(\_:amplitude:frequency:)

Sets the mode to vibrate when the user depresses the trigger at the start position or at a greater value.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
func setModeVibrationWithStartPosition(
    _ startPosition: Float,
    amplitude: Float,
    frequency: Float
)
```

## Parameters 

`startPosition`  

The effect’s start position. A value between `0` and `1` , where `0` is the minimum and `1` is the maximum trigger depression.

`amplitude`  

The amplitude of the vibration effect. A value between `0` and `1`, where `0` is the minimum and `1` is the maximum amplitude.

`frequency`  

The frequency of the vibration effect, which is a value between `0` and `1`, where `0` is the minimum and `1` is the maximum frequency.

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

func setModeVibration(amplitudes: GCDualSenseAdaptiveTrigger.PositionalAmplitudes, frequency: Float)

Sets the mode to vibrate with the specified amplitudes for each possible trigger position.

struct PositionalAmplitudes

The amplitudes for multiple positions on a trigger.

func setModeSlopeFeedback(startPosition: Float, endPosition: Float, startStrength: Float, endStrength: Float)

Sets the mode to provide feedback when the user tilts the trigger between the start and the end positions.

