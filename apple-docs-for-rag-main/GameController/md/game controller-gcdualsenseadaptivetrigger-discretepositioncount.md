

- Game Controller
- GCDualSenseAdaptiveTrigger
-  discretePositionCount 

Type Property

# discretePositionCount

The number of discrete control positions that the DualSense adaptive triggers support.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
class var discretePositionCount: Int { get }
```

## Discussion

You can configure each of these positions separately in multiposition feedback and vibration modes.

## See Also

### Related Documentation

func setModeFeedback(resistiveStrengths: GCDualSenseAdaptiveTrigger.PositionalResistiveStrengths)

Sets the mode to provide feedback with the specified strengths for each possible trigger position.

func setModeVibration(amplitudes: GCDualSenseAdaptiveTrigger.PositionalAmplitudes, frequency: Float)

Sets the mode to vibrate with the specified amplitudes for each possible trigger position.

### Getting the arm position

var armPosition: Float

The position of the trigger’s arm.

