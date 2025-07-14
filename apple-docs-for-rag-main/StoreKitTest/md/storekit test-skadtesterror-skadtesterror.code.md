

- StoreKit Test
- SKAdTestError
-  SKAdTestError.Code 

Enumeration

# SKAdTestError.Code

Enumerated error codes related to ad network testing in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
enum Code
```

## Topics

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

case signatureVerificationFailed

The signature verification failed in the testing environment.

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

case signatureVerificationFailed

The signature verification failed in the testing environment.

### Postback Errors

case excessivePostbacks

Too many postbacks submitted to the test session.

case invalidConversionValue

The conversion value isn’t valid, in the testing environment.

case invalidPostbackURL

The URL for the postback isn’t valid, in the testing environment.

case invalidRunnerUpPostback

A non-winning postback is defined with a version prior to version 3, in the testing environment.

case invalidWinningPostbackCount

The number of winning postbacks isn’t valid, in the testing environment.

case malformedPostbacks

The postback in the testing environment is malformed.

case missingPostbacks

The testing environment doesn’t have any postbacks.

case misplacedWinnerPostback

A winning postback wasn’t found in the first position, in the testing environment.

case missingWinningPostback

The testing environment is missing a winning postback.

case noPendingPostbacks

The test session doesn’t have any pending postbacks to send.

case unlinkedWinningPostbacks

The postbacks aren’t correctly related to one another.

case excessivePostbacks

Too many postbacks submitted to the test session.

case invalidConversionValue

The conversion value isn’t valid, in the testing environment.

case invalidPostbackURL

The URL for the postback isn’t valid, in the testing environment.

case invalidRunnerUpPostback

A non-winning postback is defined with a version prior to version 3, in the testing environment.

case invalidWinningPostbackCount

The number of winning postbacks isn’t valid, in the testing environment.

case malformedPostbacks

The postback in the testing environment is malformed.

case missingPostbacks

The testing environment doesn’t have any postbacks.

case misplacedWinnerPostback

A winning postback wasn’t found in the first position, in the testing environment.

case missingWinningPostback

The testing environment is missing a winning postback.

case noPendingPostbacks

The test session doesn’t have any pending postbacks to send.

case unlinkedWinningPostbacks

The postbacks aren’t correctly related to one another.

### Other Errors

case invalidVersion

A postback contains an incorrect version number.

case invalidImpressionId

The impression ID isn’t a valid UUID string.

case invalidSourceAppAdamId

The app ID is less than zero.

case invalidSourceDomain

The source domain isn’t in the correct format.

case invalidSourceIdentifier

The postback’s identifier isn’t two, three, or four digits.

case unknownError

An unknown error occurred in the testing environment.

case invalidVersion

A postback contains an incorrect version number.

case invalidImpressionId

The impression ID isn’t a valid UUID string.

case invalidSourceAppAdamId

The app ID is less than zero.

case invalidSourceDomain

The source domain isn’t in the correct format.

case invalidSourceIdentifier

The postback’s identifier isn’t two, three, or four digits.

case unknownError

An unknown error occurred in the testing environment.

### Older Errors

case invalidCampaignId

The campaign ID isn’t an integer between one and one hundred.

case signatureMissingCampaignId

The signature is missing the campaign identifier, in the testing environment.

case conflictingSource

This error code is unused.

case invalidCampaignId

The campaign ID isn’t an integer between one and one hundred.

case signatureMissingCampaignId

The signature is missing the campaign identifier, in the testing environment.

case conflictingSource

This error code is unused.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

