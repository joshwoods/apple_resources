

- PassKit (Apple Pay and Wallet)
-  PKIssuerProvisioningExtensionPassEntry 

Class

# PKIssuerProvisioningExtensionPassEntry

An object that represents an item available to add to as a Wallet pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
class PKIssuerProvisioningExtensionPassEntry
```

## Topics

### Information for displaying an addable card

var art: CGImage

An image to that the system displays to the user when they add or select the card.

var title: String

A name for the pass that the system displays to the user when they add or select the card.

var identifier: String

A developer-defined value you use to identify the card.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKIssuerProvisioningExtensionPaymentPassEntry

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

class PKIssuerProvisioningExtensionPaymentPassEntry

An object that represents a payment card available to add as a payment pass.

