

- HomeKit
- HMHome
-  rooms 

Instance Property

# rooms

An array of the rooms created and managed by the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var rooms: [HMRoom] { get }
```

## Discussion

Each HMHome instance has an immutable default room — returned by the roomForEntireHome() method — to hold accessories that the user hasn’t assigned to a specific room. Unlike user-managed rooms, the default room doesn’t appear in the rooms array.

## See Also

### Dividing a house into rooms

func roomForEntireHome() -> HMRoom

A room that represents all parts of the home that don’t have a more specific room to represent them.

func addRoom(withName: String, completionHandler: (HMRoom?, (any Error)?) -> Void)

Creates a new room with the specified name.

func removeRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Removes a room from the home.

class HMRoom

The smallest subdivision of a home’s space.

