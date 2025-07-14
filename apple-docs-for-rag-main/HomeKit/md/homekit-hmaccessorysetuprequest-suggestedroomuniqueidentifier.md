

- HomeKit
- HMAccessorySetupRequest
-  suggestedRoomUniqueIdentifier 

Instance Property

# suggestedRoomUniqueIdentifier

The identifier corresponding to the room that the framework suggests.

iOS 15.4+iPadOS 15.4+

``` source
var suggestedRoomUniqueIdentifier: UUID? { get set }
```

## Discussion

If `nil`, then any room may be suggested. See uniqueIdentifier for more information.

## See Also

### Setting up accessorices

var homeUniqueIdentifier: UUID?

The identifier corresponding to the home that the accessory should be added to when being set up.

var payload: HMAccessorySetupPayload?

The payload to use for accessory setup.

var suggestedAccessoryName: String?

The name that the framework suggests when the user names the accessory being set up.

