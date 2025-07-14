

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.unlinkedWinningPostbacks 

Case

# SKAdTestError.Code.unlinkedWinningPostbacks

The postbacks aren’t correctly related to one another.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
case unlinkedWinningPostbacks
```

## Discussion

To create multiple winning postbacks for testing multiple conversion windows, use the winningPostbacks(withVersion:adNetworkIdentifier:sourceIdentifier:appStoreItemIdentifier:sourceAppStoreItemIdentifier:sourceDomain:fidelityType:isRedownload:postbackURL:) method.

## See Also

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

