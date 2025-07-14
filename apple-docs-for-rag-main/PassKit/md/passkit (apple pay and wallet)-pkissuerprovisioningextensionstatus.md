

- PassKit (Apple Pay and Wallet)
-  PKIssuerProvisioningExtensionStatus 

Class

# PKIssuerProvisioningExtensionStatus

An object that indicates whether there are any payment cards available to add as Wallet passes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
class PKIssuerProvisioningExtensionStatus
```

## Topics

### Creating an issuer extension provisioning status

init()

Creates a new extension-handler status object.

### Reporting pass availability

var passEntriesAvailable: Bool

A Boolean value that indicates whether a payment card is available to add to an iPhone.

var remotePassEntriesAvailable: Bool

A Boolean value that indicates whether a payment card is available to add to an Apple Watch.

### Reporting requirements for authentication

var requiresAuthentication: Bool

A Boolean value that indicates whether adding a card requires an authorization-user-interface extension provided by your app.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Returning extension status

func status(completion: (PKIssuerProvisioningExtensionStatus) -> Void)

Reports the status of your Wallet extension.

