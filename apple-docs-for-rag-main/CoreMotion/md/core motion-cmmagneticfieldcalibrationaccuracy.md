

- Core Motion
-  CMMagneticFieldCalibrationAccuracy 

Enumeration

# CMMagneticFieldCalibrationAccuracy

Indicates the calibration accuracy of a magnetic field estimate

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
enum CMMagneticFieldCalibrationAccuracy
```

## Overview

One of the `enum` constants of the `CMMagneticFieldCalibrationAccuracy` type is the value of the accuracy field of the CMCalibratedMagneticField structure returned from the magneticField property.

## Topics

### Constants

case uncalibrated

The magnetic field estimate is not calibrated.

case low

The accuracy of the magnetic field calibration is low.

case medium

The accuracy of the magnetic field calibration is medium.

case high

The accuracy of the magnetic field calibration is high.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Calibrated Magnetic Field

var magneticField: CMCalibratedMagneticField

Returns the magnetic field vector with respect to the device.

struct CMCalibratedMagneticField

Calibrated magnetic field data and an estimate of the accuracy of the calibration.

