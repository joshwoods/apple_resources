

- StoreKit
- SKPaymentQueue
-  canMakePayments() Deprecated

Type Method

# canMakePayments()

A method that indicates whether the person can make purchases.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class func canMakePayments() -> Bool
```

Deprecated

Use AppStore.canMakePayments

## Discussion

The Boolean value that this method returns is identical to the value of the type property canMakePayments in the AppStore object. For more information about using and interpreting this value, see the type property page canMakePayments.

