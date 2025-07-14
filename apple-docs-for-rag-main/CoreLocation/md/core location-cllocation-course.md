

- Core Location
- CLLocation
-  course 

Instance Property

# course

The direction in which the device is traveling, measured in degrees and relative to due north.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var course: CLLocationDirection { get }
```

## Mentioned in 

Getting heading and course information

## Discussion

Course values are measured in degrees starting at due north and continue clockwise around the compass. Thus, north is 0 degrees, east is 90 degrees, south is 180 degrees, and so on. Course values may not be available on all devices. A negative value indicates that the course information is invalid.

### Special Considerations

In iOS, this property is declared as `nonatomic`. In macOS, it is declared as `atomic`.

## See Also

### Getting speed and course information

var speed: CLLocationSpeed

The instantaneous speed of the device, measured in meters per second.

var speedAccuracy: CLLocationSpeedAccuracy

The accuracy of the speed value, measured in meters per second.

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

