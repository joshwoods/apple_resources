

- StoreKit Test
- SKAdTestError
-  unknownError 

Type Property

# unknownError

An unknown error occurred in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
static var unknownError: SKAdTestError.Code { get }
```

## See Also

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

