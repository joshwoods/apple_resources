

- Foundation
- NumberFormatter
-  locale 

Instance Property

# locale

The locale of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var locale: Locale! { get set }
```

## Discussion

The locale determines the default values for many formatter attributes, such as ISO region and language codes, currency code, calendar, system of measurement, and decimal separator.

## See Also

### Managing Localization of Numbers

var localizesFormat: Bool

Determines whether the dollar sign character (`$`), decimal separator character (`.`), and thousand separator character (`,`) are converted to appropriately localized characters as specified by the user’s localization preference.

