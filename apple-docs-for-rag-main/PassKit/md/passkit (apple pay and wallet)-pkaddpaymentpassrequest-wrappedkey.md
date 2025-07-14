

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequest
-  wrappedKey 

Instance Property

# wrappedKey

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var wrappedKey: Data? { get set }
```

## See Also

### Accessing request data

var activationData: Data?

The request’s activation data.

var encryptedPassData: Data?

An encrypted JSON file containing the sensitive information needed to add a card to Apple Pay.

var ephemeralPublicKey: Data?

The ephemeral public key used by elliptic curve cryptography (ECC).

