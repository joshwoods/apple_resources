

- HomeKit
- HMHome
-  addAccessory(\_:completionHandler:) 

Instance Method

# addAccessory(\_:completionHandler:)

Adds a new accessory to the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addAccessory(
    _ accessory: HMAccessory,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func addAccessory(_ accessory: HMAccessory) async throws
```

## Parameters 

`accessory`  

The accessory to add to the home.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

You discover accessories to add to a home using the HMAccessoryBrowser class. Newly added accessories are automatically added to the room returned by roomForEntireHome().

Important

To provide a consistent user experience, use the addAndSetupAccessories(completionHandler:) method instead.

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

