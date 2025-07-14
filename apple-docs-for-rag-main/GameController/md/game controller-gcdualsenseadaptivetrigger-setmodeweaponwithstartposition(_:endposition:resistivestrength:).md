

- Game Controller
- GCDualSenseAdaptiveTrigger
-  setModeWeaponWithStartPosition(\_:endPosition:resistiveStrength:) 

Instance Method

# setModeWeaponWithStartPosition(\_:endPosition:resistiveStrength:)

Sets the mode to provide feedback when the user depresses the trigger between the start and the end positions.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
func setModeWeaponWithStartPosition(
    _ startPosition: Float,
    endPosition: Float,
    resistiveStrength: Float
)
```

## Parameters 

`startPosition`  

The effect’s start position. A value between `0` and `1` , where `0` is the minimum and `1` is the maximum trigger depression.

`endPosition`  

The effect’s end position. A value between `0` and `1` , where `0` is the minimum and `1` is the maximum trigger depression. This value must be greater than `startPosition`.

`resistiveStrength`  

The strength of the effect. A value between `0` and `1`, where `0` is the minimum or off value, and `1` is the maximum strength.

## Discussion

When the user depresses the trigger beyond the value of the end position, it stops providing feedback, giving the user a sense of release, similar to pulling a weapon trigger.

## See Also

### Configuring the trigger

func setModeFeedbackWithStartPosition(Float, resistiveStrength: Float)

Sets the mode to provide feedback when the user depresses the trigger at the start position or at a greater value.

struct PositionalResistiveStrengths

The resistive strengths for multiple positions on a trigger.

func setModeFeedback(resistiveStrengths: GCDualSenseAdaptiveTrigger.PositionalResistiveStrengths)

Sets the mode to provide feedback with the specified strengths for each possible trigger position.

func setModeVibrationWithStartPosition(Float, amplitude: Float, frequency: Float)

Sets the mode to vibrate when the user depresses the trigger at the start position or at a greater value.

func setModeVibration(amplitudes: GCDualSenseAdaptiveTrigger.PositionalAmplitudes, frequency: Float)

Sets the mode to vibrate with the specified amplitudes for each possible trigger position.

struct PositionalAmplitudes

The amplitudes for multiple positions on a trigger.

func setModeSlopeFeedback(startPosition: Float, endPosition: Float, startStrength: Float, endStrength: Float)

Sets the mode to provide feedback when the user tilts the trigger between the start and the end positions.

