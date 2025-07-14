

- HomeKit
- HMHome
-  addAndSetupAccessories(completionHandler:) Deprecated

Instance Method

# addAndSetupAccessories(completionHandler:)

Finds and adds nearby accessories to the home.

iOS 10.0–15.4DeprecatediPadOS 10.0–15.4Deprecated

``` source
func addAndSetupAccessories(completionHandler completion: @escaping ((any Error)?) -> Void)
```

``` source
func addAndSetUpAccessories() async throws
```

Deprecated

Use -\[HMAccessorySetupManager performAccessorySetupUsingRequest:completionHandler:\] instead

## Parameters 

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Mentioned in 

Testing your app with the HomeKit Accessory Simulator

## Discussion

This method launches an interactive process that first asks the user to provide a HomeKit code for the accessories—for example, by scanning an 8-digit code, by scanning the QR code, wirelessly by holding an iPhone next to the device, or by manually entering the HomeKit code. The process then asks the user to configure the accessory’s services, naming them and placing them in rooms.

## See Also

### Managing accessories

var accessories: [HMAccessory]

The collection of accessories that are part of the home.

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

func unblockAccessory(HMAccessory, completionHandler: ((any Error)?) -> Void)

Unblocks a blocked accessory.

class HMAccessory

A home automation accessory, like a garage door opener or a thermostat.

