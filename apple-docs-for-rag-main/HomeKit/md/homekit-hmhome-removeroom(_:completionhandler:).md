

- HomeKit
- HMHome
-  removeRoom(\_:completionHandler:) 

Instance Method

# removeRoom(\_:completionHandler:)

Removes a room from the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

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

## Discussion

If the room is in a zone, this method also removes it from the zone. Any accessories in the removed room automatically move to roomForEntireHome().

## See Also

### Dividing a house into rooms

var rooms: [HMRoom]

An array of the rooms created and managed by the user.

func roomForEntireHome() -> HMRoom

A room that represents all parts of the home that don’t have a more specific room to represent them.

func addRoom(withName: String, completionHandler: (HMRoom?, (any Error)?) -> Void)

Creates a new room with the specified name.

class HMRoom

The smallest subdivision of a home’s space.

