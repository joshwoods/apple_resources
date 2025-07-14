

- Core Location
- CLLocation
-  verticalAccuracy 

Instance Property

# verticalAccuracy

The validity of the altitude values, and their estimated uncertainty, measured in meters.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var verticalAccuracy: CLLocationAccuracy { get }
```

## Discussion

A positive verticalAccuracy value represents the estimated uncertainty associated with altitude and ellipsoidalAltitude. This value is available whenever altitude values are available.

If verticalAccuracy is `0` or a negative number, altitude and ellipsoidalAltitude values are invalid. If verticalAccuracy is a postive number, altitude and ellipsoidalAltitude values are valid.

A positive verticalAccuracy value represents an uncertainty that’s approximately 68 percent, or one standard deviation, above and below the altitude values.

Note

In iOS, this property is declared as `nonatomic`. In macOS, it’s declared as `atomic`.

## See Also

### Getting the location accuracy

var horizontalAccuracy: CLLocationAccuracy

The radius of uncertainty for the location, measured in meters.

typealias CLLocationAccuracy

The accuracy of a geographical coordinate.

