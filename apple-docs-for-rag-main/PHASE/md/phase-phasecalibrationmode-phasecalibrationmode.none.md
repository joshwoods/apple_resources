

- PHASE
- PHASECalibrationMode
-  PHASECalibrationMode.none 

Case

# PHASECalibrationMode.none

An option that specifies no loudness calibration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case none
```

## Discussion

For a consistent user experience across platforms and output devices, avoid PHASECalibrationMode.none by correcting loudness with PHASECalibrationMode.absoluteSpl or PHASECalibrationMode.relativeSpl.

## See Also

### Modes

case absoluteSpl

A sound pressure level based on the current output device.

case relativeSpl

A sound pressure level that’s tuned for the device.

