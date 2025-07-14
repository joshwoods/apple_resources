

- Authentication Services
-  ASAccountAuthenticationModificationControllerDelegate 

Protocol

# ASAccountAuthenticationModificationControllerDelegate

An interface you implement for receiving success and failure statuses about modification of an account’s authentication properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
protocol ASAccountAuthenticationModificationControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Topics

### Handling Requests

func accountAuthenticationModificationController(ASAccountAuthenticationModificationController, didSuccessfullyComplete: ASAccountAuthenticationModificationRequest, userInfo: [AnyHashable : Any]?)

Tells the delegate an account modification request completed successfully.

func accountAuthenticationModificationController(ASAccountAuthenticationModificationController, didFail: ASAccountAuthenticationModificationRequest, error: any Error)

Tells the delegate an account modification request failed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling Modification Requests

func cancelRequest()

Cancels a request that the user initiated.

protocol ASAccountAuthenticationModificationControllerPresentationContextProviding

An interface you implement to coordinate presentation of the user interface when modifying an account’s authentication properties.

