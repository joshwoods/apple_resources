

- HomeKit
- HMAccessorySetupRequest
-  homeUniqueIdentifier 

Instance Property

# homeUniqueIdentifier

The identifier corresponding to the home that the accessory should be added to when being set up.

iOS 15.4+iPadOS 15.4+

``` source
var homeUniqueIdentifier: UUID? { get set }
```

## Discussion

If `nil`, then the user chooses a home. See uniqueIdentifier for more information.

## See Also

### Setting up accessorices

var payload: HMAccessorySetupPayload?

The payload to use for accessory setup.

var suggestedAccessoryName: String?

The name that the framework suggests when the user names the accessory being set up.

var suggestedRoomUniqueIdentifier: UUID?

The identifier corresponding to the room that the framework suggests.

