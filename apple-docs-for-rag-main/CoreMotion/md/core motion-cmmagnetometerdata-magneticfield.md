

- Core Motion
- CMMagnetometerData
-  magneticField 

Instance Property

# magneticField

Returns the magnetic field measured by the magnetometer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var magneticField: CMMagneticField { get }
```

## Discussion

The value of this property is the total magnetic field observed by the device which is equal to the Earth’s geomagnetic field plus bias introduced from the device itself and its surroundings.

This is the “raw” magnetic-field value, unlike the calibrated value of the magneticField property of CMDeviceMotion which filters out the bias introduced by the device and, in some cases, its surrounding fields.

## See Also

### Getting the Field Strength

struct CMMagneticField

A structure containing 3-axis magnetometer data

