

- PHASE
- PHASEGeneratorNodeDefinition
-  calibrationMode 

Instance Property

# calibrationMode

A sound pressure level strategy for loudness correction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var calibrationMode: PHASECalibrationMode { get }
```

## Discussion

The default value is PHASECalibrationMode.none. To set a value, call setCalibrationMode(calibrationMode:level:).

## See Also

### Calibrating Loudness

func setCalibrationMode(calibrationMode: PHASECalibrationMode, level: Double)

Selects a loudness correction strategy and reference level.

var level: Double

The node’s loudness.

