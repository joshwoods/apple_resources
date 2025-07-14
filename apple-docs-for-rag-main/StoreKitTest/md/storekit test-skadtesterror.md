

- StoreKit Test
-  SKAdTestError 

Structure

# SKAdTestError

An error the testing environment returns for SKAdNetwork testing errors.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
struct SKAdTestError
```

## Overview

Unit tests that call setPostbacks(_:), flushPostbacks(responses:), validateImpression(parameters:publicKey:), and validate(_:publicKey:), can throw SKAdTestError errors.

When you call the unit test methods validateImpression(parameters:publicKey:), validate(_:publicKey:), or validateWebAdImpressionPayload(_:publicKey:) to validate your ad impression, the system may return signature-related errors.

When you call setPostbacks(_:) and flushPostbacks(responses:), you may get postback-related errors.

## Topics

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

static var signatureVerificationFailed: SKAdTestError.Code

The signature verification failed in the testing environment.

### Getting Postback Errors

static var excessivePostbacks: SKAdTestError.Code

Too many postbacks submitted to the test session.

static var invalidConversionValue: SKAdTestError.Code

The conversion value isn’t valid, in the testing environment.

static var invalidPostbackURL: SKAdTestError.Code

The URL for the postback isn’t valid, in the testing environment.

static var invalidRunnerUpPostback: SKAdTestError.Code

A non-winning postback is defined with a version prior to version 3, in the testing environment.

static var invalidWinningPostbackCount: SKAdTestError.Code

The number of winning postbacks isn’t valid, in the testing environment.

static var malformedPostbacks: SKAdTestError.Code

The postback in the testing environment is malformed.

static var missingPostbacks: SKAdTestError.Code

The testing environment doesn’t have any postbacks.

static var misplacedWinnerPostback: SKAdTestError.Code

A winning postback wasn’t found in the first position, in the testing environment.

static var missingWinningPostback: SKAdTestError.Code

The testing environment is missing a winning postback.

static var noPendingPostbacks: SKAdTestError.Code

The test session doesn’t have any pending postbacks to send.

static var unlinkedWinningPostbacks: SKAdTestError.Code

The postbacks aren’t correctly related to one another.

### Getting Other Errors

static var invalidVersion: SKAdTestError.Code

A postback contains an incorrect version number.

static var invalidImpressionId: SKAdTestError.Code

The impression ID isn’t a valid UUID string.

static var invalidSourceAppAdamId: SKAdTestError.Code

The app ID is less than zero.

static var invalidSourceDomain: SKAdTestError.Code

The source domain isn’t in the correct format.

static var invalidSourceIdentifier: SKAdTestError.Code

The postback’s identifier isn’t two, three, or four digits.

static var unknownError: SKAdTestError.Code

An unknown error occurred in the testing environment.

### Getting Older Errors

These errors can occur in version 3 and earlier.

static var invalidCampaignId: SKAdTestError.Code

The campaign ID isn’t an integer between one and one hundred.

static var signatureMissingCampaignId: SKAdTestError.Code

The signature is missing the campaign identifier, in the testing environment.

static var conflictingSource: SKAdTestError.Code

This error code is unused.

### Initializing the Error Objects

enum Code

Enumerated error codes related to ad network testing in the testing environment.

### Type Properties

static var errorDomain: String

The domain of the error.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Ad impression and postback errors

let SKAdTestErrorDomain: String

A string that identifies the error domain for SKAdNetwork testing in the testing environment.

