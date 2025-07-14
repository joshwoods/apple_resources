

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.signatureVerificationFailed 

Case

# SKAdTestError.Code.signatureVerificationFailed

The signature verification failed in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
case signatureVerificationFailed
```

## Discussion

The ad impression signature isn’t valid. Check the following:

- You use the same cryptographic key-pair when you sign the ad impression and validate it in the testing environment. If you use different key pairs in these two steps, signature verification will fail. For more information about signing the ad, see Signing and providing ads. For more information about validating the ad impression in the testing environment, see validate(_:publicKey:) and validateImpression(parameters:publicKey:).

- You use the correct signature instructions for the SKAdNetwork version that your app uses.For more information about SKAdNetwork versions, see SKAdNetwork release notes.

- Your signature contains all the parameters in the correct order for the version you’re using.

- Your signature uses the correct separator character.

For more information about signatures, see Signing and providing ads.

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

case missingSignature

The signature for the ad is missing, in the testing environment.

case signatureInvalidKey

The public key isn’t a valid cryptographic key, in the testing environment.

case signatureInvalidOrder

The order of the parameters in the signature is invalid, in the testing environment.

