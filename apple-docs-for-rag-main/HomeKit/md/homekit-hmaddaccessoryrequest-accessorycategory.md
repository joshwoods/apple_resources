

- HomeKit
- HMAddAccessoryRequest
-  accessoryCategory 

Instance Property

# accessoryCategory

The category of the accessory to add.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
var accessoryCategory: HMAccessoryCategory { get }
```

## See Also

### Characterizing the Request

var home: HMHome

The home to which to add the accessory.

var accessoryName: String

The name of the accessory to add.

var requiresOwnershipToken: Bool

An indication of whether the add operation requires an ownership token.

Deprecated

var requiresSetupPayloadURL: Bool

An indication of whether the add operation requires a setup payload URL.

