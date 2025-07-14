

- HomeKit
- HMHome
-  addAndSetupAccessories(with:completionHandler:) Deprecated

Instance Method

# addAndSetupAccessories(with:completionHandler:)

Finds and adds nearby accessories to the home using a HomeKit code provided by your app.

iOS 11.3–15.0DeprecatediPadOS 11.3–15.0Deprecated

``` source
func addAndSetupAccessories(
    with payload: HMAccessorySetupPayload,
    completionHandler completion: @escaping ([HMAccessory]?, (any Error)?) -> Void
)
```

``` source
func addAndSetUpAccessories(payload: HMAccessorySetupPayload) async throws -> [HMAccessory]
```

Deprecated

Use -\[HMAccessorySetupManager performAccessorySetupUsingRequest:completionHandler:\] instead

## Discussion

Use this method to add accessories that have already been deployed (for example, accessories that have HomeKit support added as a firmware update), or accessories for which scanning a QR code would be difficult. Your app provides the accessory’s HomeKit code using a setup payload. For details on the payload’s content, please join the MFi Program.

During this process, the user assigns the accessory to a room and configures its services.

## Topics

### Defining the Setup Payload

class HMAccessorySetupPayload

A payload for authenticating a HomeKit accessory.

## See Also

### Managing accessories

var accessories: [HMAccessory]

The collection of accessories that are part of the home.

func addAndSetupAccessories(completionHandler: ((any Error)?) -> Void)

Finds and adds nearby accessories to the home.

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

