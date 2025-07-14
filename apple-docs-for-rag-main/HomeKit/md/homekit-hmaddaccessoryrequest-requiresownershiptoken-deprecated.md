

- HomeKit
- HMAddAccessoryRequest
-  requiresOwnershipToken Deprecated

Instance Property

# requiresOwnershipToken

An indication of whether the add operation requires an ownership token.

iOS 13.0–13.0DeprecatediPadOS 13.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var requiresOwnershipToken: Bool { get }
```

Deprecated

No longer supported

## Discussion

In practice, this value is always `true`.

## See Also

### Characterizing the Request

var home: HMHome

The home to which to add the accessory.

var accessoryCategory: HMAccessoryCategory

The category of the accessory to add.

var accessoryName: String

The name of the accessory to add.

var requiresSetupPayloadURL: Bool

An indication of whether the add operation requires a setup payload URL.

