

- Core Location
-  CLActivityType 

Enumeration

# CLActivityType

Constants that indicate the type of activity associated with location updates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CLActivityType
```

## Topics

### Activity types

case other

The value that indicates the app is using location manager for an unspecified activity.

case automotiveNavigation

The value that indicates positioning in an automobile following a road network.

case fitness

The value that indicates positioning during dedicated fitness sessions, such as walking workouts, running workouts, cycling workouts, and so on.

case otherNavigation

The value that indicates positioning for activities that don’t or may not adhere to roads such as cycling, scooters, trains, boats and off-road vehicles.

case airborne

The value that indicates activities in the air.

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

### Running the standard location service

func startUpdatingLocation()

Starts the generation of updates that report the user’s current location.

func stopUpdatingLocation()

Stops the generation of location updates.

func requestLocation()

Requests the one-time delivery of the user’s current location.

var pausesLocationUpdatesAutomatically: Bool

A Boolean value that indicates whether the location-manager object may pause location updates.

var allowsBackgroundLocationUpdates: Bool

A Boolean value that indicates whether the app receives location updates when running in the background.

var showsBackgroundLocationIndicator: Bool

A Boolean value that indicates whether the status bar changes its appearance when an app uses location services in the background.

var activityType: CLActivityType

The type of activity the app expects the user to typically perform while in the app’s location session.

