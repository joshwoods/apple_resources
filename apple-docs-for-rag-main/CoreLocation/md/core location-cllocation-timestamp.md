

- Core Location
- CLLocation
-  timestamp 

Instance Property

# timestamp

The time at which this location was determined.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timestamp: Date { get }
```

## Discussion

In iOS, this property is declared as `nonatomic`. In macOS, it is declared as `atomic`.

## See Also

### Getting the location attributes

var coordinate: CLLocationCoordinate2D

The geographical coordinate information.

var altitude: CLLocationDistance

The altitude above mean sea level associated with a location, measured in meters.

var ellipsoidalAltitude: CLLocationDistance

The altitude as a height above the World Geodetic System 1984 (WGS84) ellipsoid, measured in meters.

typealias CLLocationDistance

A distance in meters from an existing location.

var floor: CLFloor?

The logical floor of the building in which the user is located.

var sourceInformation: CLLocationSourceInformation?

Information about the source that provides the location.

