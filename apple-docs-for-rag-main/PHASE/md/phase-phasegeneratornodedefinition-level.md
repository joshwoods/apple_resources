

- PHASE
- PHASEGeneratorNodeDefinition
-  level 

Instance Property

# level

The node’s loudness.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var level: Double { get }
```

## Discussion

The default value is `1`. To set a value, call setCalibrationMode(calibrationMode:level:).

## See Also

### Calibrating Loudness

func setCalibrationMode(calibrationMode: PHASECalibrationMode, level: Double)

Selects a loudness correction strategy and reference level.

var calibrationMode: PHASECalibrationMode

A sound pressure level strategy for loudness correction.

