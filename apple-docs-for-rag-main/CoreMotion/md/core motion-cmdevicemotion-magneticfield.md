

- Core Motion
- CMDeviceMotion
-  magneticField 

Instance Property

# magneticField

Returns the magnetic field vector with respect to the device.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var magneticField: CMCalibratedMagneticField { get }
```

## Discussion

The CMCalibratedMagneticField returned by this property gives you the total magnetic field in the device’s vicinity without device bias. Unlike the magneticField property of the CMMagnetometerData class, these values reflect the earth’s magnetic field plus surrounding fields, minus device bias.

If the device does not have a magnetometer, the `accuracy` field of the property’s value (a CMCalibratedMagneticField structure) is CMMagneticFieldCalibrationAccuracy.uncalibrated.

## See Also

### Getting the Calibrated Magnetic Field

struct CMCalibratedMagneticField

Calibrated magnetic field data and an estimate of the accuracy of the calibration.

enum CMMagneticFieldCalibrationAccuracy

Indicates the calibration accuracy of a magnetic field estimate

