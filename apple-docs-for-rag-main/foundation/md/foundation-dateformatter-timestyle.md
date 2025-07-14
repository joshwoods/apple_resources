

- Foundation
- DateFormatter
-  timeStyle 

Instance Property

# timeStyle

The time style of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeStyle: DateFormatter.Style { get set }
```

## See Also

### Managing Formats and Styles

var dateStyle: DateFormatter.Style

The date style of the receiver.

var dateFormat: String!

The date format string used by the receiver.

func setLocalizedDateFormatFromTemplate(String)

Sets the date format from a template using the specified locale for the receiver.

class func dateFormat(fromTemplate: String, options: Int, locale: Locale?) -> String?

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a date.

