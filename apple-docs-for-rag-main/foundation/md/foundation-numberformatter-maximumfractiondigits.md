

- Foundation
- NumberFormatter
-  maximumFractionDigits 

Instance Property

# maximumFractionDigits

The maximum number of digits after the decimal separator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumFractionDigits: Int { get set }
```

## Discussion

By default, this property is set to `0`.

The following code demonstrates the effect of setting maximumFractionDigits when formatting a number:

```
var numberFormatter = NumberFormatter()

numberFormatter.maximumFractionDigits = 0 // default
numberFormatter.string(from: 123.456) // 123

numberFormatter.maximumFractionDigits = 3
numberFormatter.string(from: 123.456789) // 123.457
```

## See Also

### Configuring Integer and Fraction Digits

var minimumIntegerDigits: Int

The minimum number of digits before the decimal separator.

var maximumIntegerDigits: Int

The maximum number of digits before the decimal separator.

var minimumFractionDigits: Int

The minimum number of digits after the decimal separator.

