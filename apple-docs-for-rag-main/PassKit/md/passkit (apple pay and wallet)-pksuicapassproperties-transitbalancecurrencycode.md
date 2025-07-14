

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  transitBalanceCurrencyCode 

Instance Property

# transitBalanceCurrencyCode

The currency code associated with the balance on the pass.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 3.1+

``` source
var transitBalanceCurrencyCode: String { get }
```

## Discussion

Represent the currency code associated with transitBalance as a three-letter ISO 4217 alphabetic code. For example, US Dollars is `USD` and Japanese Yen is `JPY`.

## See Also

### Getting suica balance information

var transitBalance: NSDecimalNumber

The current usable stored value on the transit card.

var isBalanceAllowedForCommute: Bool

A Boolean value that indicates how the balance can be used.

var isLowBalanceGateNotificationEnabled: Bool

A Boolean value that determines whether the terminal provides feedback if the balance is low after a deduction.

