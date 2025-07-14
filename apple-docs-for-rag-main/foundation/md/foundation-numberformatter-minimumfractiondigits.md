

- Foundation
- NumberFormatter
-  minimumFractionDigits 

Instance Property

# minimumFractionDigits

The minimum number of digits after the decimal separator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var minimumFractionDigits: Int { get set }
```

## Discussion

By default, this property is set to `0`.

The following code demonstrates the effect of setting minimumFractionDigits when formatting a number:

```
var numberFormatter = NumberFormatter()
numberFormatter.minimumFractionDigits = 0 // default
numberFormatter.string(from: 123.456) // 123
numberFormatter.minimumFractionDigits = 5
numberFormatter.string(from: 123.456) // 123.45600
```

## See Also

### Configuring Integer and Fraction Digits

var minimumIntegerDigits: Int

The minimum number of digits before the decimal separator.

var maximumIntegerDigits: Int

The maximum number of digits before the decimal separator.

var maximumFractionDigits: Int

The maximum number of digits after the decimal separator.

