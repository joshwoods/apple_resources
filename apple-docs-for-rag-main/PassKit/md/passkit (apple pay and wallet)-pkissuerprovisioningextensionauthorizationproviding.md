

- PassKit (Apple Pay and Wallet)
-  PKIssuerProvisioningExtensionAuthorizationProviding 

Protocol

# PKIssuerProvisioningExtensionAuthorizationProviding

A protocol for a UI app extension to authorize a user to add a payment card to Wallet.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
protocol PKIssuerProvisioningExtensionAuthorizationProviding : NSObjectProtocol
```

## Overview

The principal class of your app’s authorization user interface extension target must conform to the `PKIssuerProvisioningExtensionAuthorizationProviding` protocol.

Important

Before you can add a payment card provisioning UI extension you need an entitlement from Apple. For more information on requesting an entitlement, contact apple-pay-inquiries@apple.com.

## Topics

### Providing the result of authorization

var completionHandler: ((PKIssuerProvisioningExtensionAuthorizationResult) -> Void)?

A completion handler the system calls to find the result of authorizing the addition of the payment card.

**Required**

enum PKIssuerProvisioningExtensionAuthorizationResult

A value that indicates the result of authorizing the addition of a payment card.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Extend Wallet to add issuer cards

Implementing Wallet Extensions

Support adding an issued card to Apple Pay from directly within Apple Wallet using Wallet Extensions.

class PKIssuerProvisioningExtensionHandler

An abstract superclass for an app extension to add a payment card to Wallet.

