

- HomeKit
- HMHome
-  roomForEntireHome() 

Instance Method

# roomForEntireHome()

A room that represents all parts of the home that don’t have a more specific room to represent them.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
func roomForEntireHome() -> HMRoom
```

## Return Value

The room that represents all parts of the home that don’t have a more specific room to represent them.

## Discussion

HomeKit assigns new accessories to this room until you assign them to a more specific room with assignAccessory(_:to:completionHandler:), or until the user assigns them to a room using the Home app.

You can’t rename this room, add it to a zone, or remove it from the home. It also doesn’t appear in the home’s rooms array.

## See Also

### Dividing a house into rooms

var rooms: [HMRoom]

An array of the rooms created and managed by the user.

func addRoom(withName: String, completionHandler: (HMRoom?, (any Error)?) -> Void)

Creates a new room with the specified name.

func removeRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Removes a room from the home.

class HMRoom

The smallest subdivision of a home’s space.

