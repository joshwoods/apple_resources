

- SensorKit
- SRWristTemperature
-  errorEstimate 

Instance Property

# errorEstimate

An estimate of the amount of error in the temperature measurement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var errorEstimate: Measurement { get }
```

## Discussion

This property is a delta value that can be positive or negative.

## See Also

### Getting temperature information

var timestamp: Date

The date and time when the device records the temperature.

var value: Measurement&lt;UnitTemperature>

The temperature sensor value in celsius.

