

- MapKit
-  MKUserTrackingMode 

Enumeration

# MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.2+visionOS 1.0+

``` source
enum MKUserTrackingMode
```

## Topics

### Constants

case none

The map doesn’t follow the user’s location.

case follow

The map follows the user location.

case followWithHeading

The map follows the user’s location and rotates when the heading changes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

