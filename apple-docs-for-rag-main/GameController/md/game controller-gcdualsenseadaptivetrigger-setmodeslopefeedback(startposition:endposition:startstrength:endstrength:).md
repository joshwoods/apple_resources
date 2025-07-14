

- Game Controller
- GCDualSenseAdaptiveTrigger
-  setModeSlopeFeedback(startPosition:endPosition:startStrength:endStrength:) 

Instance Method

# setModeSlopeFeedback(startPosition:endPosition:startStrength:endStrength:)

Sets the mode to provide feedback when the user tilts the trigger between the start and the end positions.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func setModeSlopeFeedback(
    startPosition: Float,
    endPosition: Float,
    startStrength: Float,
    endStrength: Float
)
```

## Parameters 

`startPosition`  

The effect’s start position, which is a value between `0` and `1` , where `0` is the minimum and `1` is the maximum trigger tilt.

`endPosition`  

The effect’s end position, which is a value between `0` and `1` , where `0` is the minimum and `1` is the maximum trigger tilt. This value must be greater than `startPosition`.

`startStrength`  

The effect’s start strength, which is a value between `0` and `1`, where `0` is the minimum or off value, and `1` is the maximum strength.

`endStrength`  

The effect’s end strength, which is a value between `0` and `1`, where `0` is the minimum or off value, and `1` is the maximum strength.

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

struct PositionalAmplitudes

The amplitudes for multiple positions on a trigger.

