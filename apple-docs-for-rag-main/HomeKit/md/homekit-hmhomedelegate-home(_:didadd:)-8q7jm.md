

- HomeKit
- HMHomeDelegate
-  home(\_:didAdd:) 

Instance Method

# home(\_:didAdd:)

Tells the delegate that a home added a user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func home(
    _ home: HMHome,
    didAdd user: HMUser
)
```

## Parameters 

`home`  

The home.

`user`  

The user that was added.

## See Also

### Observing Home Configuration

func homeDidUpdateName(HMHome)

Tells the delegate that a home’s name changed.

func home(HMHome, didAdd: HMAccessory)

Tells the delegate that a home added a new accessory.

func home(HMHome, didUpdate: HMRoom, for: HMAccessory)

Tells the delegate that a home assigned an accessory to a different room.

func home(HMHome, didRemove: HMAccessory)

Tells the delegate that a home removed an accessory.

func home(HMHome, didAdd: HMRoom)

Tells the delegate that a home added a new room.

func home(HMHome, didUpdateNameFor: HMRoom)

Tells the delegate that a home updated the name of one of its rooms.

func home(HMHome, didAdd: HMRoom, to: HMZone)

Tells the delegate that a home added a room to a zone.

func home(HMHome, didRemove: HMRoom, from: HMZone)

Tells the delegate that a home removed a room from a zone.

func home(HMHome, didRemove: HMRoom)

Tells the delegate that a home removed a room.

func home(HMHome, didAdd: HMZone)

Tells the delegate that a home added a new zone.

func home(HMHome, didUpdateNameFor: HMZone)

Tells the delegate that a home changed the name of a zone.

func home(HMHome, didRemove: HMZone)

Tells the delegate that a home removed a zone.

func home(HMHome, didRemove: HMUser)

Tells the delegate that a home removed a user.

func homeDidUpdateAccessControl(forCurrentUser: HMHome)

Tells the delegate that the access control for the current user has changed.

func home(HMHome, didUpdate: HMHomeHubState)

Tells the delegate that the state of the home hub has changed.

