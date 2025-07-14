

- PassKit (Apple Pay and Wallet)
- PKTransitPassProperties
-  transitBalanceCurrencyCode Deprecated

Instance Property

# transitBalanceCurrencyCode

The currency code associated with the balance on the pass.

iOS 11.3–15.0DeprecatediPadOS 11.3–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 11.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.3–8.0Deprecated

``` source
var transitBalanceCurrencyCode: String { get }
```

## Discussion

Represent the currency code associated with transitBalance as a three-letter ISO 4217 alphabetic code. For example, US Dollars is `USD` and Japanese Yen is `JPY`.

## See Also

### Getting balance information

var transitBalance: NSDecimalNumber

The current usable stored value on the transit card.

Deprecated

