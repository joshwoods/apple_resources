

- PassKit (Apple Pay and Wallet)
-  PKAddPaymentPassRequest 

Class

# PKAddPaymentPassRequest

Contains the card data needed to add a card to Apple Pay.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
class PKAddPaymentPassRequest
```

## Overview

All sensitive data must be encrypted before being assigned to this object. Because the encryption keys vary depending on the server, create PKAddPaymentPassRequest instances only when your PKAddPaymentPassViewControllerDelegate object’s addPaymentPassViewController(_:generateRequestWithCertificateChain:nonce:nonceSignature:completionHandler:) method is called. The required server certificates are provided at that time.

Important

Adding payment passes requires a special entitlement issued by Apple. Your app must include this entitlement before you can use this class. For more information on requesting this entitlement, see the Card Issuers section at developer.apple.com/apple-pay/.

## Topics

### Creating an add payment pass request

init()

### Accessing request data

var activationData: Data?

The request’s activation data.

var encryptedPassData: Data?

An encrypted JSON file containing the sensitive information needed to add a card to Apple Pay.

var ephemeralPublicKey: Data?

The ephemeral public key used by elliptic curve cryptography (ECC).

var wrappedKey: Data?

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

### Requesting to add payment cards to Apple Pay

func addPaymentPassViewController(PKAddPaymentPassViewController, generateRequestWithCertificateChain: [Data], nonce: Data, nonceSignature: Data, completionHandler: (PKAddPaymentPassRequest) -> Void)

Asks the delegate to create an add payment request.

**Required**

func addPaymentPassViewController(PKAddPaymentPassViewController, didFinishAdding: PKPaymentPass?, error: (any Error)?)

**Required**

