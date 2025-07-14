

- HomeKit
- HMAddAccessoryRequest
-  home 

Instance Property

# home

The home to which to add the accessory.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
var home: HMHome { get }
```

## Discussion

Call this home’s addAndSetupAccessories(with:completionHandler:) method to fulfill the request after constructing the setup payload.

## See Also

### Characterizing the Request

var accessoryCategory: HMAccessoryCategory

The category of the accessory to add.

var accessoryName: String

The name of the accessory to add.

var requiresOwnershipToken: Bool

An indication of whether the add operation requires an ownership token.

Deprecated

var requiresSetupPayloadURL: Bool

An indication of whether the add operation requires a setup payload URL.

