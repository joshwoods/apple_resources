

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.signatureInvalidKey 

Case

# SKAdTestError.Code.signatureInvalidKey

The public key isn’t a valid cryptographic key, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
case signatureInvalidKey
```

## Discussion

The public key that you provide in the validate(_:publicKey:) or validateImpression(parameters:publicKey:) methods must be a key that uses Elliptic Curve Digital Signature Algorithm (ECDSA) with a prime256v1 curve. For more information about the key, see Registering an ad network.

## See Also

### Signature Errors

case missingSignature

The signature for the ad is missing, in the testing environment.

case signatureInvalidOrder

The order of the parameters in the signature is invalid, in the testing environment.

case signatureMissingAdNetworkId

The signature is missing an ad network identifier, in the testing environment.

case signatureMissingAppAdamId

The signature is missing the app item identifier for the advertised app, in the testing environment.

case signatureMissingFidelityType

The signature is missing the fidelity type, in the testing environment.

case signatureMissingNonce

The signature is missing the nonce, in the testing environment.

case signatureMissingSourceAppAdamId

The signature is missing the source app item identifier, in the testing environment.

case signatureMissingSourceDomain

The signature is missing the source domain, in the testing environment.

case signatureMissingSourceIdentifier

The signature is missing the source identifier, in the testing environment.

case signatureMissingTimestamp

The signature is missing a timestamp, in the testing environment.

case signatureUnknownError

An unknown error occurred with the signature in the testing environment.

case signatureVerificationFailed

The signature verification failed in the testing environment.

case missingSignature

The signature for the ad is missing, in the testing environment.

case signatureInvalidOrder

The order of the parameters in the signature is invalid, in the testing environment.

case signatureMissingAdNetworkId

The signature is missing an ad network identifier, in the testing environment.

