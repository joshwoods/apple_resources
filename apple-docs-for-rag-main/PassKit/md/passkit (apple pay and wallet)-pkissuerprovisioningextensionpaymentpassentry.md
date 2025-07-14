

- PassKit (Apple Pay and Wallet)
-  PKIssuerProvisioningExtensionPaymentPassEntry 

Class

# PKIssuerProvisioningExtensionPaymentPassEntry

An object that represents a payment card available to add as a payment pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
class PKIssuerProvisioningExtensionPaymentPassEntry
```

## Topics

### Creating a payment pass entry

init?(identifier: String, title: String, art: CGImage, addRequestConfiguration: PKAddPaymentPassRequestConfiguration)

Creates a new entry for a payment pass that a user adds to Wallet.

### Getting the pass entry configuration

var addRequestConfiguration: PKAddPaymentPassRequestConfiguration

The configuration that the system uses to add a payment pass.

## Relationships

### Inherits From

- PKIssuerProvisioningExtensionPassEntry

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Returning available passes

func passEntries(completion: ([PKIssuerProvisioningExtensionPassEntry]) -> Void)

Reports the list of passes available to add to an iPhone.

func remotePassEntries(completion: ([PKIssuerProvisioningExtensionPassEntry]) -> Void)

Reports the list of passes available to add to an Apple Watch.

class PKIssuerProvisioningExtensionPassEntry

An object that represents an item available to add to as a Wallet pass.

