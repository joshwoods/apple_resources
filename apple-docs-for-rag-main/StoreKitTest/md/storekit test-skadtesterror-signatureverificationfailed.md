

- StoreKit Test
- SKAdTestError
-  signatureVerificationFailed 

Type Property

# signatureVerificationFailed

The signature verification failed in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
static var signatureVerificationFailed: SKAdTestError.Code { get }
```

## Discussion

The ad impression signature isn’t valid. Check the following:

- You use the same cryptographic key-pair when you sign the ad impression and validate it in the testing environment. If you use different key pairs in these two steps, signature verification will fail. For more information about signing the ad, see Signing and providing ads. For more information about validating the ad impression in the testing environment, see validate(_:publicKey:) and validateImpression(parameters:publicKey:).

- You use the correct signature instructions for the SKAdNetwork version that your app uses. For more information about SKAdNetwork versions, see SKAdNetwork release notes.

- Your signature contains all the parameters in the correct order for the version you’re using.

- Your signature uses the correct separator character.

For more information about signatures, see Signing and providing ads.

## See Also

### Getting Signature Errors

static var missingSignature: SKAdTestError.Code

The signature for the ad is missing, in the testing environment.

static var signatureInvalidKey: SKAdTestError.Code

The public key isn’t a valid cryptographic key, in the testing environment.

static var signatureInvalidOrder: SKAdTestError.Code

The order of the parameters in the signature is invalid, in the testing environment.

static var signatureMissingAdNetworkId: SKAdTestError.Code

The signature is missing an ad network identifier, in the testing environment.

static var signatureMissingAppAdamId: SKAdTestError.Code

The signature is missing the app item identifier for the advertised app, in the testing environment.

static var signatureMissingFidelityType: SKAdTestError.Code

The signature is missing the fidelity type, in the testing environment.

static var signatureMissingNonce: SKAdTestError.Code

The signature is missing the nonce, in the testing environment.

static var signatureMissingSourceAppAdamId: SKAdTestError.Code

The signature is missing the source app item identifier, in the testing environment.

static var signatureMissingSourceDomain: SKAdTestError.Code

The signature is missing the source domain, in the testing environment.

static var signatureMissingSourceIdentifier: SKAdTestError.Code

The signature is missing the source identifier, in the testing environment.

static var signatureMissingTimestamp: SKAdTestError.Code

The signature is missing a timestamp, in the testing environment.

static var signatureUnknownError: SKAdTestError.Code

An unknown error occurred with the signature in the testing environment.

