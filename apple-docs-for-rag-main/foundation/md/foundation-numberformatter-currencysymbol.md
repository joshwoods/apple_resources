

- Foundation
- NumberFormatter
-  currencySymbol 

Instance Property

# currencySymbol

The string used by the receiver as a local currency symbol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var currencySymbol: String! { get set }
```

## Discussion

A region typically has a local currency symbol and an international currency symbol. The local symbol is used within the region, while the international currency symbol is used in international contexts to specify that region’s currency unambiguously. The local currency symbol is often represented by a Unicode code point.

## See Also

### Configuring the Format of Currency

var currencyCode: String!

The receiver’s currency code.

var internationalCurrencySymbol: String!

The international currency symbol used by the receiver.

var currencyGroupingSeparator: String!

The currency grouping separator for the receiver.

