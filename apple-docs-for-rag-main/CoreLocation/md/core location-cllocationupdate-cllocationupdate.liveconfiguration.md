

- Core Location
- CLLocationUpdate
-  CLLocationUpdate.LiveConfiguration 

Enumeration

# CLLocationUpdate.LiveConfiguration

Values for indicating the kind of updates the framework delivers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum LiveConfiguration
```

## Topics

### Location types

case `default`

The value that configures positioning for activities that one of the other activity types doesn’t cover.

case airborne

The value that configures positioning for activities in the air.

case automotiveNavigation

The value that configures positioning for an automobile following a road network.

case fitness

The value that configures positioning for dedicated fitness sessions.

case otherNavigation

The value that configures positioning for transportation that doesn’t, or may not, adhere to roads, such as cycling, scooters, trains, boats, and off-road vehicles.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Receiving location updates

static func liveUpdates(CLLocationUpdate.LiveConfiguration) -> CLLocationUpdate.Updates

Tells Core Location to start delivering the location updates it produces for the configuration you specify.

struct Updates

A structure that represents an asynchronous sequence of location updates.

