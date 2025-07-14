

- PHASE
- PHASEGeneratorNodeDefinition
-  setCalibrationMode(calibrationMode:level:) 

Instance Method

# setCalibrationMode(calibrationMode:level:)

Selects a loudness correction strategy and reference level.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func setCalibrationMode(
    calibrationMode: PHASECalibrationMode,
    level: Double
)
```

## Parameters 

`calibrationMode`  

A given strategy for sound pressure level. For a consistent user experience across platforms and output devices, choose PHASECalibrationMode.absoluteSpl or PHASECalibrationMode.relativeSpl.

`level`  

The loudness. The calibration mode determines this value’s unit and range.

## See Also

### Calibrating Loudness

var calibrationMode: PHASECalibrationMode

A sound pressure level strategy for loudness correction.

var level: Double

The node’s loudness.

