

- StoreKit Test
- SKAdTestError
-  signatureInvalidKey 

Type Property

# signatureInvalidKey

The public key isn’t a valid cryptographic key, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
static var signatureInvalidKey: SKAdTestError.Code { get }
```

## Discussion

The public key that you provide in the validate(_:publicKey:) or validateImpression(parameters:publicKey:) methods must be a key that uses Elliptic Curve Digital Signature Algorithm (ECDSA) with a prime256v1 curve. For more information about the key, see Registering an ad network.

## See Also

### Getting Signature Errors

static var missingSignature: SKAdTestError.Code

The signature for the ad is missing, in the testing environment.

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

static var signatureVerificationFailed: SKAdTestError.Code

The signature verification failed in the testing environment.

