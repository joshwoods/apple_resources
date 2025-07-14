

- HomeKit
- HMHome
-  unblockAccessory(\_:completionHandler:) 

Instance Method

# unblockAccessory(\_:completionHandler:)

Unblocks a blocked accessory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func unblockAccessory(
    _ accessory: HMAccessory,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func unblockAccessory(_ accessory: HMAccessory) async throws
```

## Parameters 

`accessory`  

The accessory to unblock.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

A misbehaving accessory automatically becomes blocked. After that, all requests to the accessory fail. Use this API to explicitly unblock the accessory.

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

var supportsAddingNetworkRouter: Bool

A Boolean that indicates whether a home supports all of the requirements for adding a network router.

class HMAccessory

A home automation accessory, like a garage door opener or a thermostat.

