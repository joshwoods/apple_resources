

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequest
-  encryptedPassData 

Instance Property

# encryptedPassData

An encrypted JSON file containing the sensitive information needed to add a card to Apple Pay.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var encryptedPassData: Data? { get set }
```

## Discussion

The JSON file must contain the following keys:

| Key | Type | Description |
|----|----|----|
| primaryAccountNumber | String | The full primary account number (PAN). Digits only. |
| expiration | String | The expiration date as a string. For example, `"11/18"`. |
| name | String | The name of the card holder. |
| nonce | String | The hex string for the nonce value, provided in the delegate callback. |
| nonceSignature | String | The hex string for the nonce signature, provided in the delegate callback. |

## See Also

### Accessing request data

var activationData: Data?

The request’s activation data.

var ephemeralPublicKey: Data?

The ephemeral public key used by elliptic curve cryptography (ECC).

var wrappedKey: Data?

