

- Foundation
- Decimal
- Decimal.FormatStyle
-  init(locale:) 

Initializer

# init(locale:)

Creates a decimal format style that uses the given locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(locale: Locale = .autoupdatingCurrent)
```

## Parameters 

`locale`  

The locale to use when formatting or parsing decimal values. Defaults to autoupdatingCurrent.

## Discussion

Create a Decimal.FormatStyle instance when you intend to apply a given style to multiple decimal values. The following example creates a style that uses the `en_US` locale, which uses three-based grouping and comma separators. It then applies this style to all the Decimal values in an array.

```
let enUSstyle = Decimal.FormatStyle(locale: Locale(identifier: "en_US"))
let decimals: [Decimal] = [100.1, 1000.2, 10000.3, 100000.4, 1000000.5]
let formattedDecimals = decimals.map { enUSstyle.format($0) } // ["100.1", "1,000.2", "10,000.3", "100,000.4", "1,000,000.5"]
```

To format a single integer, you can use the Decimal instance method formatted(_:) passing in an instance of Decimal.FormatStyle.

