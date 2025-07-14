

- PassKit (Apple Pay and Wallet)
-  PKAddPaymentPassViewControllerDelegate 

Protocol

# PKAddPaymentPassViewControllerDelegate

Methods that let the system prompt you for an add payment request, and inform you when a request has succeeded or failed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
protocol PKAddPaymentPassViewControllerDelegate : NSObjectProtocol
```

## Overview

Delegates for the PKAddPaymentPassViewController class must adopt this protocol.

Important

Adding payment passes requires a special entitlement issued by Apple. Your app must include this entitlement before you can use this class. For more information on requesting this entitlement, see the Card Issuers section at developer.apple.com/apple-pay/.

## Topics

### Requesting to add payment cards to Apple Pay

func addPaymentPassViewController(PKAddPaymentPassViewController, generateRequestWithCertificateChain: [Data], nonce: Data, nonceSignature: Data, completionHandler: (PKAddPaymentPassRequest) -> Void)

Asks the delegate to create an add payment request.

**Required**

class PKAddPaymentPassRequest

Contains the card data needed to add a card to Apple Pay.

func addPaymentPassViewController(PKAddPaymentPassViewController, didFinishAdding: PKPaymentPass?, error: (any Error)?)

**Required**

### Payment pass errors

enum PKAddPaymentPassError

Error codes for adding payment passes.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working with add payment view controllers

var delegate: (any PKAddPaymentPassViewControllerDelegate)?

The object that acts as the delegate for the add payment view controller.

