

- Core Location
- CLLocation
-  speed 

Instance Property

# speed

The instantaneous speed of the device, measured in meters per second.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var speed: CLLocationSpeed { get }
```

## Mentioned in 

Getting heading and course information

## Discussion

This value reflects the instantaneous speed of the device as it moves in the direction of its current heading. A negative value indicates an invalid speed. Because the actual speed can change many times between the delivery of location events, use this property for informational purposes only.

### Special Considerations

In iOS, this property is declared as `nonatomic`. In macOS, it is declared as `atomic`.

## See Also

### Getting speed and course information

var speedAccuracy: CLLocationSpeedAccuracy

The accuracy of the speed value, measured in meters per second.

var course: CLLocationDirection

The direction in which the device is traveling, measured in degrees and relative to due north.

var courseAccuracy: CLLocationDirectionAccuracy

The accuracy of the course value, measured in degrees.

typealias CLLocationSpeed

The velocity (measured in meters per second) at which the device is moving.

typealias CLLocationDirection

An azimuth that is measured in degrees relative to true north.

typealias CLLocationSpeedAccuracy

The accuracy of a speed.

typealias CLLocationDirectionAccuracy

The accuracy of a compass heading.

