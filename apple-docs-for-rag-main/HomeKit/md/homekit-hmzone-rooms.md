

- HomeKit
- HMZone
-  rooms 

Instance Property

# rooms

Array of rooms in the zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var rooms: [HMRoom] { get }
```

## See Also

### Assigning Rooms to a Zone

func addRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Adds a room to the zone.

func removeRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Removes a room from the zone.

