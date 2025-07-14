

- PassKit (Apple Pay and Wallet)
-  PKIssuerProvisioningExtensionHandler 

Class

# PKIssuerProvisioningExtensionHandler

An abstract superclass for an app extension to add a payment card to Wallet.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class PKIssuerProvisioningExtensionHandler
```

## Overview

The principal class of your app’s extension target must be a subclass of `PKIssuerProvisioningExtensionHandler`.

Your app must be installed and the user open the app at least once for the system to call the extension handler.

Important

Before you can add a payment card provisioning extension you need an entitlement from Apple. For more information on requesting an entitlement, contact apple-pay-inquiries@apple.com.

## Topics

### Returning extension status

func status(completion: (PKIssuerProvisioningExtensionStatus) -> Void)

Reports the status of your Wallet extension.

class PKIssuerProvisioningExtensionStatus

An object that indicates whether there are any payment cards available to add as Wallet passes.

### Returning available passes

func passEntries(completion: ([PKIssuerProvisioningExtensionPassEntry]) -> Void)

Reports the list of passes available to add to an iPhone.

func remotePassEntries(completion: ([PKIssuerProvisioningExtensionPassEntry]) -> Void)

Reports the list of passes available to add to an Apple Watch.

class PKIssuerProvisioningExtensionPassEntry

An object that represents an item available to add to as a Wallet pass.

class PKIssuerProvisioningExtensionPaymentPassEntry

An object that represents a payment card available to add as a payment pass.

### Returning information for adding a pass

func generateAddPaymentPassRequestForPassEntryWithIdentifier(String, configuration: PKAddPaymentPassRequestConfiguration, certificateChain: [Data], nonce: Data, nonceSignature: Data, completionHandler: (PKAddPaymentPassRequest?) -> Void)

Creates an object with the data the system needs to add a card to Apple Pay.

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

### Extend Wallet to add issuer cards

Implementing Wallet Extensions

Support adding an issued card to Apple Pay from directly within Apple Wallet using Wallet Extensions.

protocol PKIssuerProvisioningExtensionAuthorizationProviding

A protocol for a UI app extension to authorize a user to add a payment card to Wallet.

