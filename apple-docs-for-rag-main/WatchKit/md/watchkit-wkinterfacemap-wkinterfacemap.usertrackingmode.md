

- WatchKit
- WKInterfaceMap
-  WKInterfaceMap.UserTrackingMode 

Enumeration

# WKInterfaceMap.UserTrackingMode

Modes for tracking the user’s location on the map.

watchOS 6.1+

``` source
enum UserTrackingMode
```

## Topics

### Tracking Modes

case follow

The map scrolls to follow the user as they move.

case none

The map remains stationary, even if the user moves off the map.

case follow

The map scrolls to follow the user as they move.

case none

The map remains stationary, even if the user moves off the map.

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

### Displaying the User’s Location

func setShowsUserLocation(Bool)

Sets whether the map shows the user’s current location.

func setShowsUserHeading(Bool)

Sets whether the map shows the user heading.

func setUserTrackingMode(WKInterfaceMap.UserTrackingMode, animated: Bool)

Sets the map’s tracking mode.

