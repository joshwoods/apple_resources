

- Core Location
- CLLocation
-  floor 

Instance Property

# floor

The logical floor of the building in which the user is located.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var floor: CLFloor? { get }
```

## Discussion

If floor information is not available for the current location, the value of this property is `nil`.

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

var timestamp: Date

The time at which this location was determined.

var sourceInformation: CLLocationSourceInformation?

Information about the source that provides the location.

