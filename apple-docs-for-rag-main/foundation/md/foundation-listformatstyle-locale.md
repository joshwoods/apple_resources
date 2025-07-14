

- Foundation
- ListFormatStyle
-  locale 

Instance Property

# locale

The locale to use when formatting items in the list.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var locale: Locale
```

## Discussion

A Locale instance is typically used to provide, format, and interpret information about and according to the user’s customs and preferences.

Examples include ISO region and language codes, currency code, calendar, system of measurement, and decimal separator.

The default value is autoupdatingCurrent. If you set this property to `nil`, the formatter resets to using `autoupdatingCurrent`.

## See Also

### Modifying a list format style

var width: ListFormatStyle&lt;Style, Base>.Width

The size of the list.

enum Width

The type representing the width of a list.

var listType: ListFormatStyle&lt;Style, Base>.ListType

The type of the list.

enum ListType

A type that describes whether the returned list contains cumulative or alternative elements.

