

- HomeKit
- HMAddAccessoryRequest
-  requiresSetupPayloadURL 

Instance Property

# requiresSetupPayloadURL

An indication of whether the add operation requires a setup payload URL.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
var requiresSetupPayloadURL: Bool { get }
```

## Discussion

If this value is `true`, look up the URL for the given accessory based on its category and name, given by the request’s accessoryCategory and accessoryName parameters. Include the URL in the setup payload by calling the request’s makePayload(url:ownershipToken:) method.

If requiresSetupPayloadURL is `false`, you can still use the makePayload(url:ownershipToken:) method, if appropriate. Alternatively, you can construct the payload by calling the request’s makePayload(ownershipToken:) command instead.

## See Also

### Characterizing the Request

var home: HMHome

The home to which to add the accessory.

var accessoryCategory: HMAccessoryCategory

The category of the accessory to add.

var accessoryName: String

The name of the accessory to add.

var requiresOwnershipToken: Bool

An indication of whether the add operation requires an ownership token.

Deprecated

