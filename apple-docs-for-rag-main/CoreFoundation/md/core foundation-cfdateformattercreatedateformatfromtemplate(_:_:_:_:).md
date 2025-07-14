

- Core Foundation
-  CFDateFormatterCreateDateFormatFromTemplate(\_:\_:\_:\_:) 

Function

# CFDateFormatterCreateDateFormatFromTemplate(\_:\_:\_:\_:)

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFDateFormatterCreateDateFormatFromTemplate(
    _ allocator: CFAllocator!,
    _ tmplate: CFString!,
    _ options: CFOptionFlags,
    _ locale: CFLocale!
) -> CFString!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`tmplate`  

A string containing date format patterns (such as “MM” or “h”). For full details, see Unicode Technical Standard #35.

`options`  

No options are currently defined—pass `0`.

`locale`  

The locale for which the template is required.

## Return Value

A localized date format string representing the date format components given in `template`, arranged appropriately for the locale specified by `locale`. Ownership follows the The Create Rule.

## Discussion

The returned string may not contain exactly those components given in `template`, but may—for example—have locale-specific adjustments applied.

## Discussion

Different locales have different conventions for the ordering of date components. You use this method to get an appropriate format string for a given set of components for a specified locale (typically you use the current locale—see CFLocaleCopyCurrent()).

The following example shows the difference between the date formats for British and American English:

```
CFStringRef dateComponents = CFSTR("yMMMMd");

CFLocaleRef usLocale = CFLocaleCreate(NULL, CFSTR("en_US"));
CFStringRef usDateFormatString =
    CFDateFormatterCreateDateFormatFromTemplate(NULL, dateComponents, 0, usLocale);
// Date format for English (United States): MMMM d, y

CFLocaleRef gbLocale = CFLocaleCreate(NULL, CFSTR("en_GB"));
CFStringRef gbDateFormatString =
    CFDateFormatterCreateDateFormatFromTemplate(NULL, dateComponents, 0, gbLocale);
// Date format for English (United Kingdom): d MMMM y
```

## See Also

### Creating Strings From Data

func CFDateFormatterCreateStringWithAbsoluteTime(CFAllocator!, CFDateFormatter!, CFAbsoluteTime) -> CFString!

Returns a string representation of the given absolute time using the specified date formatter.

func CFDateFormatterCreateStringWithDate(CFAllocator!, CFDateFormatter!, CFDate!) -> CFString!

Returns a string representation of the given date using the specified date formatter.

