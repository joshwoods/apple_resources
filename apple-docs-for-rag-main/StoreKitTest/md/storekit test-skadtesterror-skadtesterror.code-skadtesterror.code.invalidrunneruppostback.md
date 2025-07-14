

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.invalidRunnerUpPostback 

Case

# SKAdTestError.Code.invalidRunnerUpPostback

A non-winning postback is defined with a version prior to version 3, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
case invalidRunnerUpPostback
```

## Discussion

Check that all non-winning postback you create with init(version:adNetworkIdentifier:adCampaignIdentifier:appStoreItemIdentifier:sourceAppStoreItemIdentifier:conversionValue:fidelityType:isRedownload:didWin:postbackURL:) in SKAdTestPostback specify version 3 (version3_0) or later. Non-winning postbacks are available starting in version 3. For more information about versions, see SKAdNetwork release notes.

## See Also

### Postback Errors

case excessivePostbacks

Too many postbacks submitted to the test session.

case invalidConversionValue

The conversion value isn’t valid, in the testing environment.

case invalidPostbackURL

The URL for the postback isn’t valid, in the testing environment.

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

case invalidWinningPostbackCount

The number of winning postbacks isn’t valid, in the testing environment.

case malformedPostbacks

The postback in the testing environment is malformed.

