

- HomeKit
- HMHome
-  addRoom(withName:completionHandler:) 

Instance Method

# addRoom(withName:completionHandler:)

Creates a new room with the specified name.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addRoom(
    withName roomName: String,
    completionHandler completion: @escaping (HMRoom?, (any Error)?) -> Void
)
```

``` source
func addRoom(named roomName: String) async throws -> HMRoom
```

## Parameters 

`roomName`  

The name of the new room. Must not be `nil`, and must not be the name of a room already in the home.

`completion`  

The block executed after the request is processed.

room  
The newly created room.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Dividing a house into rooms

var rooms: [HMRoom]

An array of the rooms created and managed by the user.

func roomForEntireHome() -> HMRoom

A room that represents all parts of the home that don’t have a more specific room to represent them.

func removeRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Removes a room from the home.

class HMRoom

The smallest subdivision of a home’s space.

