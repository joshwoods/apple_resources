

- Core Motion
- CMOdometerData
-  maxAbsSlope 

Instance Property

# maxAbsSlope

The maximum absolute slope at the location toward all directions, measured in degrees.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 10.15+visionOS 1.0+watchOS 8.4+

``` source
var maxAbsSlope: Double? { get }
```

## Discussion

If the maximum absolute slope is invalid due to low GPS accuracy, this property is nil.

## See Also

### Getting speed and slope

var speed: CLLocationSpeed

The instantaneous velocity of the device, measured in meters per second.

var slope: Double?

The slope at the location toward the direction of travel, measured in degrees.

