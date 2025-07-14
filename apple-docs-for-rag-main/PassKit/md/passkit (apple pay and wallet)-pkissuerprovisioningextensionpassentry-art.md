

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionPassEntry
-  art 

Instance Property

# art

An image to that the system displays to the user when they add or select the card.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
var art: CGImage { get }
```

## Discussion

The image requirements are:

- Square corners.

- Doesn’t include an account number.

- Doesn’t include the user name.

## See Also

### Information for displaying an addable card

var title: String

A name for the pass that the system displays to the user when they add or select the card.

var identifier: String

A developer-defined value you use to identify the card.

