

- Core Location
- CLHeading
-  headingAccuracy 

Instance Property

# headingAccuracy

The maximum deviation (measured in degrees) between the reported heading and the true geomagnetic heading.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+watchOS 2.0+

``` source
var headingAccuracy: CLLocationDirection { get }
```

## Discussion

A positive value in this property represents the potential error between the value reported by the magneticHeading property and the actual direction of magnetic north. Thus, the lower the value of this property, the more accurate the heading. A negative value means that the reported heading is invalid, which can occur when the device is uncalibrated or there is strong interference from local magnetic fields.

## See Also

### Getting the heading values

var magneticHeading: CLLocationDirection

The heading (measured in degrees) relative to magnetic north.

var trueHeading: CLLocationDirection

The heading (measured in degrees) relative to true north.

