

- HomeKit
- HMZone
-  removeRoom(\_:completionHandler:) 

Instance Method

# removeRoom(\_:completionHandler:)

Removes a room from the zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func removeRoom(
    _ room: HMRoom,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeRoom(_ room: HMRoom) async throws
```

## Parameters 

`room`  

The room to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Assigning Rooms to a Zone

var rooms: [HMRoom]

Array of rooms in the zone.

func addRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Adds a room to the zone.

