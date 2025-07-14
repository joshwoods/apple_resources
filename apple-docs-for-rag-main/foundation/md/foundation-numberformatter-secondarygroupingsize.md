

- Foundation
- NumberFormatter
-  secondaryGroupingSize 

Instance Property

# secondaryGroupingSize

The secondary grouping size of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var secondaryGroupingSize: Int { get set }
```

## Discussion

Some locales allow the specification of another grouping size for larger numbers. For example, some locales may represent a number such as 61, 242, 378.46 (as in the United States) as 6,12,42,378.46. In this case, the secondary grouping size (covering the groups of digits furthest from the decimal point) is 2.

## See Also

### Configuring Separators and Grouping Size

var groupingSeparator: String!

The string used by the receiver for a grouping separator.

var usesGroupingSeparator: Bool

Determines whether the receiver displays the group separator.

var thousandSeparator: String!

The character the receiver uses as a thousand separator.

var hasThousandSeparators: Bool

Determines whether the receiver uses thousand separators.

var decimalSeparator: String!

The character the receiver uses as a decimal separator.

var alwaysShowsDecimalSeparator: Bool

Determines whether the receiver always shows the decimal separator, even for integer numbers.

var currencyDecimalSeparator: String!

The string used by the receiver as a currency decimal separator.

var groupingSize: Int

The grouping size of the receiver.

