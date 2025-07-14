

- Core Location
- CLLocation
-  courseAccuracy 

Instance Property

# courseAccuracy

The accuracy of the course value, measured in degrees.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+

``` source
var courseAccuracy: CLLocationDirectionAccuracy { get }
```

## Discussion

When this property contains `0` or a positive number, the value in the course property is plus or minus the specified number degrees, modulo 360. When this property contains a negative number, the value in the course property is invalid.

## See Also

### Getting speed and course information

var speed: CLLocationSpeed

The instantaneous speed of the device, measured in meters per second.

var speedAccuracy: CLLocationSpeedAccuracy

The accuracy of the speed value, measured in meters per second.

var course: CLLocationDirection

The direction in which the device is traveling, measured in degrees and relative to due north.

typealias CLLocationSpeed

The velocity (measured in meters per second) at which the device is moving.

typealias CLLocationDirection

An azimuth that is measured in degrees relative to true north.

typealias CLLocationSpeedAccuracy

The accuracy of a speed.

typealias CLLocationDirectionAccuracy

The accuracy of a compass heading.

