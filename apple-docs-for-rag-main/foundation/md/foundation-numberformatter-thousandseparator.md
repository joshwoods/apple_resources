

- Foundation
- NumberFormatter
-  thousandSeparator 

Instance Property

# thousandSeparator

The character the receiver uses as a thousand separator.

macOS 10.0+

``` source
var thousandSeparator: String! { get set }
```

## Discussion

If you don’t have thousand separators enabled through any other means (such as format), using this method enables them.

### Special Considerations

This method is for use with formatters using `NSNumberFormatterBehavior10_0` behavior.

## See Also

### Configuring Separators and Grouping Size

var groupingSeparator: String!

The string used by the receiver for a grouping separator.

var usesGroupingSeparator: Bool

Determines whether the receiver displays the group separator.

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

var secondaryGroupingSize: Int

The secondary grouping size of the receiver.

