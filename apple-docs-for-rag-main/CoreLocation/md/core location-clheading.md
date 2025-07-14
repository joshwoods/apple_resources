

- Core Location
-  CLHeading 

Class

# CLHeading

The orientation of the user’s device, relative to true or magnetic north.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+watchOS 2.0+

``` source
class CLHeading
```

## Overview

A CLHeading object contains computed values for the device’s azimuth (orientation) relative to true or magnetic north. It also includes the raw data for the three-dimensional vector used to compute those values. A navigation app might use the information to rotate a map so that it reflects the direction that the user is facing.

Typically, you don’t create instances of this class yourself, nor do you subclass it. Instead, you receive instances of this class through the delegate assigned to the CLLocationManager object whose startUpdatingHeading() method you called.

Note

If you want heading objects to contain valid data for the trueHeading property, configure your location manager object to deliver location updates. You can start the delivery of these updates by calling the location manager object’s startUpdatingLocation() method.

## Topics

### Getting the heading values

var magneticHeading: CLLocationDirection

The heading (measured in degrees) relative to magnetic north.

var trueHeading: CLLocationDirection

The heading (measured in degrees) relative to true north.

var headingAccuracy: CLLocationDirection

The maximum deviation (measured in degrees) between the reported heading and the true geomagnetic heading.

### Getting the raw heading data

var x: CLHeadingComponentValue

The geomagnetic data (measured in microteslas) for the x-axis.

var y: CLHeadingComponentValue

The geomagnetic data (measured in microteslas) for the y-axis.

var z: CLHeadingComponentValue

The geomagnetic data (measured in microteslas) for the z-axis.

typealias CLHeadingComponentValue

A type used to report magnetic differences reported by the onboard hardware.

### Getting the event timestamp

var timestamp: Date

The time at which this heading was determined.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Compass headings

Getting heading and course information

Use a device’s orientation and course information for navigation.

