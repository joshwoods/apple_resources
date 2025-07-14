

- HomeKit
- HMHome
-  supportsAddingNetworkRouter 

Instance Property

# supportsAddingNetworkRouter

A Boolean that indicates whether a home supports all of the requirements for adding a network router.

iOS 13.2+iPadOS 13.2+tvOS 13.2+visionOS 1.0+watchOS 6.1+

``` source
var supportsAddingNetworkRouter: Bool { get }
```

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

func assignAccessory(HMAccessory, to: HMRoom, completionHandler: ((any Error)?) -> Void)

Assigns an accessory to a different room.

func removeAccessory(HMAccessory, completionHandler: ((any Error)?) -> Void)

Removes an accessory from the home.

func unblockAccessory(HMAccessory, completionHandler: ((any Error)?) -> Void)

Unblocks a blocked accessory.

class HMAccessory

A home automation accessory, like a garage door opener or a thermostat.

