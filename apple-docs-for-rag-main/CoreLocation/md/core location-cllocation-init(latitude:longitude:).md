

- Core Location
- CLLocation
-  init(latitude:longitude:) 

Initializer

# init(latitude:longitude:)

Creates a location object with the specified latitude and longitude.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    latitude: CLLocationDegrees,
    longitude: CLLocationDegrees
)
```

## Parameters 

`latitude`  

The latitude of the geographical coordinate.

`longitude`  

The longitude of the geographical coordinate.

## Return Value

A location object initialized with the specified geographical coordinate.

## Discussion

Use this method to create location objects that are not necessarily based on the user’s current location. Typically, you acquire location objects from your CLLocationManager object, which returns the user’s actual location. However, you might use this method when you want to represent any location on a map. For example, you might create an object to represent the user’s intended destination.

This method records the latitude and longitude values you provide, and it initializes other properties to appropriate default values. Specifically, this method sets the altitude and horizontalAccuracy properties to 0, sets the verticalAccuracy property to `-1` to indicate that the altitude is invalid, sets the speed and course values to `-1`, and sets the timestamp property to the time at which the returned object was created.

## See Also

### Creating a location object

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, timestamp: Date)

Creates a location object with the specified coordinate and altitude information.

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, course: CLLocationDirection, speed: CLLocationSpeed, timestamp: Date)

Creates a location object with the specified coordinate, altitude, and course information.

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, course: CLLocationDirection, courseAccuracy: CLLocationDirectionAccuracy, speed: CLLocationSpeed, speedAccuracy: CLLocationSpeedAccuracy, timestamp: Date)

Creates a location object with the specified coordinate, altitude, course, and accuracy information.

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, course: CLLocationDirection, courseAccuracy: CLLocationDirectionAccuracy, speed: CLLocationSpeed, speedAccuracy: CLLocationSpeedAccuracy, timestamp: Date, sourceInfo: CLLocationSourceInformation)

