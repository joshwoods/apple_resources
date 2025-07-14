

- Foundation
- NumberFormatter
-  minimumIntegerDigits 

Instance Property

# minimumIntegerDigits

The minimum number of digits before the decimal separator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var minimumIntegerDigits: Int { get set }
```

## Discussion

By default, this property is set to `0`.

The following code demonstrates the effect of setting minimumIntegerDigits when formatting a number:

```
var numberFormatter = NumberFormatter()

numberFormatter.minimumIntegerDigits = 0 // default
numberFormatter.string(from: 123) // 123

numberFormatter.minimumIntegerDigits = 5
numberFormatter.string(from: 123) // 00123
```

## See Also

### Configuring Integer and Fraction Digits

var maximumIntegerDigits: Int

The maximum number of digits before the decimal separator.

var minimumFractionDigits: Int

The minimum number of digits after the decimal separator.

var maximumFractionDigits: Int

The maximum number of digits after the decimal separator.

