

- StoreKit Test
- SKTestSession
-  failureError Deprecated

Instance Property

# failureError

The error code that transactions return when you enable failing transactions.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedwatchOS 7.0–10.0Deprecated

``` source
var failureError: SKError.Code { get set }
```

Deprecated

No longer supported. Use simulatedError(forAPI:)

## Discussion

You can force an error by setting failTransactionsEnabled to `true` and setting failureError value to one of these supported error codes: SKError.Code.unknown, SKError.Code.invalidOfferIdentifier, SKError.Code.invalidSignature, SKError.Code.missingOfferParams, SKError.Code.invalidOfferPrice.

Use these settings to test your how your app responds to failed transactions.

## See Also

### Forcing failed transactions

var failTransactionsEnabled: Bool

A Boolean value that determines whether transactions fail in the testing environment.

Deprecated

