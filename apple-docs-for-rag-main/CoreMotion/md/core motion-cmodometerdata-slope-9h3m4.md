

- Core Motion
- CMOdometerData
-  slope 

Instance Property

# slope

The slope at the location toward the direction of travel, measured in degrees.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 10.15+visionOS 1.0+watchOS 8.4+

``` source
var slope: Double? { get }
```

## Discussion

If the slope measurement is invalid, this property is nil.

## See Also

### Getting speed and slope

var speed: CLLocationSpeed

The instantaneous velocity of the device, measured in meters per second.

var maxAbsSlope: Double?

The maximum absolute slope at the location toward all directions, measured in degrees.

