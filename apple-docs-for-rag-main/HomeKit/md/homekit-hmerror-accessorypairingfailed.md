

- HomeKit
- HMError
-  accessoryPairingFailed 

Type Property

# accessoryPairingFailed

An attempt to pair with the accessory has failed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var accessoryPairingFailed: HMError.Code { get }
```

## See Also

### Detecting communication errors

static var accessDenied: HMError.Code

An error indicating the current user doesn’t have privileges to perform the operation.

static var accessoryCommunicationFailure: HMError.Code

The accessory failed to communicate.

static var accessorySentInvalidResponse: HMError.Code

An error indicating the accessory sent an invalid response.

static var clientRequestError: HMError.Code

An error with the client request.

static var communicationFailure: HMError.Code

A communication failure.

static var dataResetFailure: HMError.Code

An attempt to reset the data failed.

static var timedOutWaitingForAccessory: HMError.Code

An accessory did not respond timely.

static var partialCommunicationFailure: HMError.Code

