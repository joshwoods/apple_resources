

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.malformedPostbacks 

Case

# SKAdTestError.Code.malformedPostbacks

The postback in the testing environment is malformed.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
case malformedPostbacks
```

## Discussion

Check that all parameters in the postback use the correct type.

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

