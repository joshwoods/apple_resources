

- HomeKit
- HMHome
-  assignAccessory(\_:to:completionHandler:) 

Instance Method

# assignAccessory(\_:to:completionHandler:)

Assigns an accessory to a different room.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func assignAccessory(
    _ accessory: HMAccessory,
    to room: HMRoom,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func assignAccessory(
    _ accessory: HMAccessory,
    to room: HMRoom
) async throws
```

## Parameters 

`accessory`  

The accessory to assign; must already have been added to the home.

`room`  

The room to which the accessory will be assigned; must already exist in the home.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Managing accessories

var accessories: [HMAccessory]

The collection of accessories that are part of the home.

func addAndSetupAccessories(completionHandler: ((any Error)?) -> Void)

Finds and adds nearby accessories to the home.

Deprecated

func addAndSetupAccessories(with: HMAccessorySetupPayload, completionHandler: ([HMAccessory]?, (any Error)?) -> Void)

Finds and adds nearby accessories to the home using a HomeKit code provided by your app.

Deprecated

func addAccessory(HMAccessory, completionHandler: ((any Error)?) -> Void)

Adds a new accessory to the home.

func removeAccessory(HMAccessory, completionHandler: ((any Error)?) -> Void)

Removes an accessory from the home.

var supportsAddingNetworkRouter: Bool

A Boolean that indicates whether a home supports all of the requirements for adding a network router.

func unblockAccessory(HMAccessory, completionHandler: ((any Error)?) -> Void)

Unblocks a blocked accessory.

class HMAccessory

A home automation accessory, like a garage door opener or a thermostat.

