

- Foundation
- DateFormatter
-  dateFormat(fromTemplate:options:locale:) 

Type Method

# dateFormat(fromTemplate:options:locale:)

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func dateFormat(
    fromTemplate tmplate: String,
    options opts: Int,
    locale: Locale?
) -> String?
```

## Parameters 

`tmplate`  

A string containing date format patterns (such as “MM” or “h”).

For full details, see Date and Time Programming Guide.

`opts`  

No options are currently defined.

`locale`  

The locale for which the template is required.

## Return Value

A localized date format string representing the date format components given in `template`, arranged appropriately for the locale specified by `locale`.

## Discussion

The returned string may not contain exactly those components given in `template`, but may—for example—have locale-specific adjustments applied.

## Discussion

Different locales have different conventions for the ordering of date components. You use this method to get an appropriate format string for a given set of components for a specified locale (typically you use the current locale—see current).

The following example shows the difference between the date formats for British and American English:

- Swift
- Objective-C

```
let usLocale = Locale(identifier: "en_US")
let gbLocale = Locale(identifier: "en_GB")
let template = "yMMMMd"

let usDateFormat = DateFormatter.dateFormat(fromTemplate: template, options: 0, locale: usLocale)!
// Date format for English (United States): "MMMM d, y"
let gbDateFormat = DateFormatter.dateFormat(fromTemplate: template, options: 0, locale: gbLocale)!
// Date format for English (United Kingdom): "d MMMM y"
```

```
NSLocale *usLocale = [[NSLocale alloc] initWithLocaleIdentifier:@"en_US"];
NSLocale *gbLocale = [[NSLocale alloc] initWithLocaleIdentifier:@"en_GB"];

NSString *template = @"yMMMMd";

NSString *enDateFormat = [NSDateFormatter dateFormatFromTemplate:template options:0 locale:usLocale];
NSLog(@"Date format for %@: %@",
    [usLocale displayNameForKey:NSLocaleIdentifier value:[usLocale localeIdentifier]], enDateFormat);

NSString *gbDateFormat = [NSDateFormatter dateFormatFromTemplate:template options:0 locale:gbLocale];
NSLog(@"Date format for %@: %@",
    [gbLocale displayNameForKey:NSLocaleIdentifier value:[gbLocale localeIdentifier]], gbDateFormat);

// Output:
// Date format for English (United States): MMMM d, y
// Date format for English (United Kingdom): d MMMM y
```

## See Also

### Managing Formats and Styles

var dateStyle: DateFormatter.Style

The date style of the receiver.

var timeStyle: DateFormatter.Style

The time style of the receiver.

var dateFormat: String!

The date format string used by the receiver.

func setLocalizedDateFormatFromTemplate(String)

Sets the date format from a template using the specified locale for the receiver.

var formattingContext: Formatter.Context

The capitalization formatting context used when formatting a date.

