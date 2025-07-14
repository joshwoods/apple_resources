

- HomeKit
- HMZone
-  addRoom(\_:completionHandler:) 

Instance Method

# addRoom(\_:completionHandler:)

Adds a room to the zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func addRoom(
    _ room: HMRoom,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func addRoom(_ room: HMRoom) async throws
```

## Parameters 

`room`  

The room to add; must be in the same home as the zone.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Assigning Rooms to a Zone

var rooms: [HMRoom]

Array of rooms in the zone.

func removeRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Removes a room from the zone.

