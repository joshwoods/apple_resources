

- Core Motion
- CMAbsoluteAltitudeData
-  altitude 

Instance Property

# altitude

The absolute altitude of the device relative to sea level, measured in meters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
var altitude: Double { get }
```

## Discussion

This value can be positive or negative.

## See Also

### Accessing Altitude Data

var accuracy: Double

The estimated uncertainty of the altimeter in meters, based on one standard deviation.

var precision: Double

The recommended resolution for the altitude, in meters.

