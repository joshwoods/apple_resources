

- HomeKit
- HMAccessorySetupRequest
-  payload 

Instance Property

# payload

The payload to use for accessory setup.

iOS 15.4+iPadOS 15.4+

``` source
@NSCopying
var payload: HMAccessorySetupPayload? { get set }
```

## Discussion

See HMAccessorySetupPayload for more information.

## See Also

### Setting up accessorices

var homeUniqueIdentifier: UUID?

The identifier corresponding to the home that the accessory should be added to when being set up.

var suggestedAccessoryName: String?

The name that the framework suggests when the user names the accessory being set up.

var suggestedRoomUniqueIdentifier: UUID?

The identifier corresponding to the room that the framework suggests.

