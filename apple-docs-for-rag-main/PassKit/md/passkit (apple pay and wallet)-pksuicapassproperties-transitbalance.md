

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  transitBalance 

Instance Property

# transitBalance

The current usable stored value on the transit card.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 3.1+

``` source
@NSCopying
var transitBalance: NSDecimalNumber { get }
```

## See Also

### Getting suica balance information

var transitBalanceCurrencyCode: String

The currency code associated with the balance on the pass.

var isBalanceAllowedForCommute: Bool

A Boolean value that indicates how the balance can be used.

var isLowBalanceGateNotificationEnabled: Bool

A Boolean value that determines whether the terminal provides feedback if the balance is low after a deduction.

