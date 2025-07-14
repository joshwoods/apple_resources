

- Core Foundation
-  CFDateFormatterCreate(\_:\_:\_:\_:) 

Function

# CFDateFormatterCreate(\_:\_:\_:\_:)

Creates a new CFDateFormatter object, localized to the given locale, which will format dates to the given date and time styles.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterCreate(
    _ allocator: CFAllocator!,
    _ locale: CFLocale!,
    _ dateStyle: CFDateFormatterStyle,
    _ timeStyle: CFDateFormatterStyle
) -> CFDateFormatter!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`locale`  

The locale to use for localization. If `NULL` uses the default system local. Use CFLocaleCopyCurrent() to specify the locale of the current user.

`dateStyle`  

The date style to use when formatting dates. See Date Formatter Styles for possible values.

`timeStyle`  

The time style to use when formatting times. See Date Formatter Styles for possible values.

## Return Value

A new date formatter, localized to the given locale, which will format dates to the given date and time styles. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

You can use `kCFDateFormatterNoStyle` to suppress output for the date or time. The following code fragment illustrates the creation and use of a date formatter that only outputs the date information (memory management is omitted for clarity).

```
CFLocaleRef locale = CFLocaleCreate(kCFAllocatorDefault, CFSTR("en_GB"));

CFDateFormatterRef formatter = CFDateFormatterCreate(
        kCFAllocatorDefault, locale, kCFDateFormatterMediumStyle, kCFDateFormatterNoStyle);

CFDateRef date = CFDateCreate(kCFAllocatorDefault, 123456);
CFStringRef dateAsString = CFDateFormatterCreateStringWithDate (
        kCFAllocatorDefault, formatter, date);

CFShow(dateAsString);
// outputs "2 Jan 2001"
```

