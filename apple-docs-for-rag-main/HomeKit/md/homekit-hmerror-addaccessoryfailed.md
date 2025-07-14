

- HomeKit
- HMError
-  addAccessoryFailed 

Type Property

# addAccessoryFailed

A failed attempt to add an accessory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var addAccessoryFailed: HMError.Code { get }
```

## See Also

### Detecting accessory errors

static var accessoryIsBlocked: HMError.Code

An error indicating a blocked accessory.

static var accessoryIsBusy: HMError.Code

An error indicating the accessory is busy.

static var accessoryIsSuspended: HMError.Code

The accessory is suspended.

static var accessoryNotReachable: HMError.Code

An error indicating the accessory is not reachable over the network.

static var accessoryOutOfCompliance: HMError.Code

An error indicating the accessory is out of compliance.

static var accessoryOutOfResources: HMError.Code

An error indicating the accessory is out of resources.

static var accessoryPoweredOff: HMError.Code

An error indicating the accessory is off.

static var accessoryResponseError: HMError.Code

An error with the accessory’s response.

static var incompatibleAccessory: HMError.Code

The accessory is incompatible.

