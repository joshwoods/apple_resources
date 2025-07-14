

- Foundation
- DateFormatter
-  setLocalizedDateFormatFromTemplate(\_:) 

Instance Method

# setLocalizedDateFormatFromTemplate(\_:)

Sets the date format from a template using the specified locale for the receiver.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setLocalizedDateFormatFromTemplate(_ dateFormatTemplate: String)
```

## Parameters 

`dateFormatTemplate`  

A string containing date format patterns (such as “MM” or “h”).

For full details, see Date and Time Programming Guide.

## Discussion

See Data Formatting Guide for a list of the conversion specifiers permitted in date format strings.

Calling this method is equivalent to, but not necessarily implemented as, setting the dateFormat property to the result of calling the dateFormat(fromTemplate:options:locale:) method, passing no options and the locale property value.

Important

You should call this method only after setting the locale of the receiver.

## See Also

### Related Documentation

var locale: Locale!

The locale for the receiver.

### Managing Formats and Styles

var dateStyle: DateFormatter.Style

The date style of the receiver.

var timeStyle: DateFormatter.Style

The time style of the receiver.

var dateFormat: String!

The date format string used by the receiver.

class func dateFormat(fromTemplate: String, options: Int, locale: Locale?) -> String?

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a date.

