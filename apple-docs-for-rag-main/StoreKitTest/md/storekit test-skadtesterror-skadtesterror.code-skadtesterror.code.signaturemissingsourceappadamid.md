

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.signatureMissingSourceAppAdamId 

Case

# SKAdTestError.Code.signatureMissingSourceAppAdamId

The signature is missing the source app item identifier, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
case signatureMissingSourceAppAdamId
```

## Discussion

Be sure to include the app item identifier for the source app when you create and validate an ad impression in the testing environment.

## See Also

### Signature Errors

case missingSignature

The signature for the ad is missing, in the testing environment.

case signatureInvalidKey

The public key isn’t a valid cryptographic key, in the testing environment.

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

case signatureInvalidKey

The public key isn’t a valid cryptographic key, in the testing environment.

case signatureInvalidOrder

The order of the parameters in the signature is invalid, in the testing environment.

