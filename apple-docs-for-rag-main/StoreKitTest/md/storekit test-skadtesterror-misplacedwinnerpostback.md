

- StoreKit Test
- SKAdTestError
-  misplacedWinnerPostback 

Type Property

# misplacedWinnerPostback

A winning postback wasn’t found in the first position, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
static var misplacedWinnerPostback: SKAdTestError.Code { get }
```

## Discussion

Check that the first postback in the `postbacks` array you provide to setPostbacks(_:) is marked as a winning postback, with `didWin` set to `true`. Check that the winning postback is in no other position in the array.

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

static var missingWinningPostback: SKAdTestError.Code

The testing environment is missing a winning postback.

static var noPendingPostbacks: SKAdTestError.Code

The test session doesn’t have any pending postbacks to send.

static var unlinkedWinningPostbacks: SKAdTestError.Code

The postbacks aren’t correctly related to one another.

