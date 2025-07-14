

- Authentication Services
-  ASAccountAuthenticationModificationControllerPresentationContextProviding 

Protocol

# ASAccountAuthenticationModificationControllerPresentationContextProviding

An interface you implement to coordinate presentation of the user interface when modifying an account’s authentication properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
protocol ASAccountAuthenticationModificationControllerPresentationContextProviding : NSObjectProtocol
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Topics

### Presenting the Account Modification Interface

func presentationAnchor(for: ASAccountAuthenticationModificationController) -> ASPresentationAnchor

Returns the most appropriate window for presenting the authentication modification interface.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling Modification Requests

func cancelRequest()

Cancels a request that the user initiated.

protocol ASAccountAuthenticationModificationControllerDelegate

An interface you implement for receiving success and failure statuses about modification of an account’s authentication properties.

