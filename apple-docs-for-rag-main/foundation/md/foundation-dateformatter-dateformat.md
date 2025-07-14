

- Foundation
- DateFormatter
-  dateFormat 

Instance Property

# dateFormat

The date format string used by the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dateFormat: String! { get set }
```

## Discussion

See Data Formatting Guide for a list of the conversion specifiers permitted in date format strings.

You should only set this property when working with fixed format representations, as discussed in Working With Fixed Format Date Representations. For user-visible representations, you should use the dateStyle and timeStyle properties, or the setLocalizedDateFormatFromTemplate(_:) method if your desired format cannot be achieved using the predefined styles; both of these properties and this method provide a localized date representation appropriate for display to the user.

## See Also

### Managing Formats and Styles

var dateStyle: DateFormatter.Style

The date style of the receiver.

var timeStyle: DateFormatter.Style

The time style of the receiver.

func setLocalizedDateFormatFromTemplate(String)

Sets the date format from a template using the specified locale for the receiver.

class func dateFormat(fromTemplate: String, options: Int, locale: Locale?) -> String?

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a date.

