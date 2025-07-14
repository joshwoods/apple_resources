

- StoreKit Test
- SKTestSession
-  failTransactionsEnabled Deprecated

Instance Property

# failTransactionsEnabled

A Boolean value that determines whether transactions fail in the testing environment.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedwatchOS 7.0–10.0Deprecated

``` source
var failTransactionsEnabled: Bool { get set }
```

Deprecated

No longer supported. Use simulatedError(forAPI:)

## Discussion

The default value is `false`. Set this value to `true` when you want to test your app’s response to SKPaymentTransaction transactions that fail. Attempted transactions in the payment queue show the SKPaymentTransactionState.failed state, with the error code that you set in failureError.

Changing this property overrides its setting in the StoreKit configuration file for this test session. Call resetToDefaultState() to revert all settings to those in the configuration file.

## See Also

### Forcing failed transactions

var failureError: SKError.Code

The error code that transactions return when you enable failing transactions.

Deprecated

