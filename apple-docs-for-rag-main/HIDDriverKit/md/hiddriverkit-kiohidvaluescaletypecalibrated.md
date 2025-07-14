

- HIDDriverKit
-  kIOHIDValueScaleTypeCalibrated 

Enumeration Case

# kIOHIDValueScaleTypeCalibrated

An option to scale the value with respect to a set of calibration properties.

DriverKitmacOS

``` source
kIOHIDValueScaleTypeCalibrated
```

## Discussion

The system sets calibration properties for some types of data. For example, the built-in event driver calibrates digitizer data to the logical minimum and maximum values. If no calibration properties are set, the getScaledValue method calibrates the value to the range `-1` to `1`.

## See Also

### Getting the Options

kIOHIDValueScaleTypePhysical

An option to scale the value with respect to the physical minimum and maximum values.

kIOHIDValueScaleTypeExponent

An option to scale the value with respect to the element’s unit exponent.

