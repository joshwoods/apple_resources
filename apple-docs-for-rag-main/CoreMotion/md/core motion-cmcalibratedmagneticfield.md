

- Core Motion
-  CMCalibratedMagneticField 

Structure

# CMCalibratedMagneticField

Calibrated magnetic field data and an estimate of the accuracy of the calibration.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
struct CMCalibratedMagneticField
```

## Topics

### Initializers

init()

Initializes the magnetic field to a set of default values.

init(field: CMMagneticField, accuracy: CMMagneticFieldCalibrationAccuracy)

Initializes the magnetic field to the specified set of values.

### Accessing the Field Values

var field: CMMagneticField

A structure containing 3-axis calibrated magnetic field data. See the description of the CMMagneticField structure.

var accuracy: CMMagneticFieldCalibrationAccuracy

An enum-constant value that indicates the accuracy of the magnetic field estimate. See CMMagneticFieldCalibrationAccuracy.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting the Calibrated Magnetic Field

var magneticField: CMCalibratedMagneticField

Returns the magnetic field vector with respect to the device.

enum CMMagneticFieldCalibrationAccuracy

Indicates the calibration accuracy of a magnetic field estimate

