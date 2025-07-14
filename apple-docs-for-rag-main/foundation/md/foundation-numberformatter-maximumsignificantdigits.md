

- Foundation
- NumberFormatter
-  maximumSignificantDigits 

Instance Property

# maximumSignificantDigits

The maximum number of significant digits for the number formatter.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumSignificantDigits: Int { get set }
```

## Discussion

You must set the usesSignificantDigits property to true in order for this property to affect formatting behavior. By default, the maximum number of significant digits is 6. Values less than 1 are ignored.

The following code demonstrates the effect of setting maximumSignificantDigits when formatting various numbers:

```
var numberFormatter = NumberFormatter()
numberFormatter.usesSignificantDigits = true
numberFormatter.maximumSignificantDigits = 4

numberFormatter.string(from: 12345) // 12340
numberFormatter.string(from: 123.456) // 123.5
numberFormatter.string(from: 100.234) // 100.2
numberFormatter.string(from: 1.230) // 1.23
numberFormatter.string(from: 0.00012345) // 0.0001234
```

## See Also

### Configuring Significant Digits

var usesSignificantDigits: Bool

A Boolean value indicating whether the formatter uses minimum and maximum significant digits when formatting numbers.

var minimumSignificantDigits: Int

The minimum number of significant digits for the number formatter.

