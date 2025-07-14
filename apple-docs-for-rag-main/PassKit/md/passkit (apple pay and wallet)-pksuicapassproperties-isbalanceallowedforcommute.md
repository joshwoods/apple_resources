

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  isBalanceAllowedForCommute 

Instance Property

# isBalanceAllowedForCommute

A Boolean value that indicates how the balance can be used.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 4.3+

``` source
var isBalanceAllowedForCommute: Bool { get }
```

## Discussion

The Suica network determines the value and usage of this property.

## See Also

### Getting suica balance information

var transitBalance: NSDecimalNumber

The current usable stored value on the transit card.

var transitBalanceCurrencyCode: String

The currency code associated with the balance on the pass.

var isLowBalanceGateNotificationEnabled: Bool

A Boolean value that determines whether the terminal provides feedback if the balance is low after a deduction.

