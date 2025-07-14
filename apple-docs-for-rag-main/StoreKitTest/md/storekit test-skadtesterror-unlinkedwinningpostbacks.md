

- StoreKit Test
- SKAdTestError
-  unlinkedWinningPostbacks 

Type Property

# unlinkedWinningPostbacks

The postbacks aren’t correctly related to one another.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
static var unlinkedWinningPostbacks: SKAdTestError.Code { get }
```

## Discussion

To create linked winning postbacks for testing multiple conversion windows, use the winningPostbacks(withVersion:adNetworkIdentifier:sourceIdentifier:appStoreItemIdentifier:sourceAppStoreItemIdentifier:sourceDomain:fidelityType:isRedownload:postbackURL:) method.

## See Also

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

