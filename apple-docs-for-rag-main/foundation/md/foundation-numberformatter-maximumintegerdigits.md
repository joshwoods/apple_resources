

- Foundation
- NumberFormatter
-  maximumIntegerDigits 

Instance Property

# maximumIntegerDigits

The maximum number of digits before the decimal separator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumIntegerDigits: Int { get set }
```

## Discussion

By default, this property is set to `42`.

The following code demonstrates the effect of setting maximumIntegerDigits when formatting a number:

```
var numberFormatter = NumberFormatter()

numberFormatter.maximumIntegerDigits = 42 // default
numberFormatter.string(from: 12345) // 12345

numberFormatter.maximumIntegerDigits = 3
numberFormatter.string(from: 12345) // 345
```

## See Also

### Configuring Integer and Fraction Digits

var minimumIntegerDigits: Int

The minimum number of digits before the decimal separator.

var minimumFractionDigits: Int

The minimum number of digits after the decimal separator.

var maximumFractionDigits: Int

The maximum number of digits after the decimal separator.

