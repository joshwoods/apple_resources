

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequest
-  activationData 

Instance Property

# activationData

The request’s activation data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var activationData: Data? { get set }
```

## Discussion

This property contains the data provided to the payment network as a cryptographic one-time pad (OTP), per the Payment Network API specification. The cryptographic OTP is not interpreted by Apple or iOS. The OTP should be verified by the issuer and/or payment network upon receipt of the provisioning request to ensure the request’s authenticity. For more information about the activation data’s content, contact your payment network.

Note

This is the same type of activation data that is accepted by the pass library’s activate(_:withActivationData:completion:) method.

## See Also

### Accessing request data

var encryptedPassData: Data?

An encrypted JSON file containing the sensitive information needed to add a card to Apple Pay.

var ephemeralPublicKey: Data?

The ephemeral public key used by elliptic curve cryptography (ECC).

var wrappedKey: Data?

