

- Core Location
- CLLocation
-  init(coordinate:altitude:horizontalAccuracy:verticalAccuracy:course:courseAccuracy:speed:speedAccuracy:timestamp:sourceInfo:) 

Initializer

# init(coordinate:altitude:horizontalAccuracy:verticalAccuracy:course:courseAccuracy:speed:speedAccuracy:timestamp:sourceInfo:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    coordinate: CLLocationCoordinate2D,
    altitude: CLLocationDistance,
    horizontalAccuracy hAccuracy: CLLocationAccuracy,
    verticalAccuracy vAccuracy: CLLocationAccuracy,
    course: CLLocationDirection,
    courseAccuracy: CLLocationDirectionAccuracy,
    speed: CLLocationSpeed,
    speedAccuracy: CLLocationSpeedAccuracy,
    timestamp: Date,
    sourceInfo: CLLocationSourceInformation
)
```

## See Also

### Creating a location object

init(latitude: CLLocationDegrees, longitude: CLLocationDegrees)

Creates a location object with the specified latitude and longitude.

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, timestamp: Date)

Creates a location object with the specified coordinate and altitude information.

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, course: CLLocationDirection, speed: CLLocationSpeed, timestamp: Date)

Creates a location object with the specified coordinate, altitude, and course information.

init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance, horizontalAccuracy: CLLocationAccuracy, verticalAccuracy: CLLocationAccuracy, course: CLLocationDirection, courseAccuracy: CLLocationDirectionAccuracy, speed: CLLocationSpeed, speedAccuracy: CLLocationSpeedAccuracy, timestamp: Date)

Creates a location object with the specified coordinate, altitude, course, and accuracy information.

