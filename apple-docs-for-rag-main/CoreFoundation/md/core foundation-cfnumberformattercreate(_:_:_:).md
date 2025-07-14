

- Core Foundation
-  CFNumberFormatterCreate(\_:\_:\_:) 

Function

# CFNumberFormatterCreate(\_:\_:\_:)

Creates a new CFNumberFormatter object, localized to the given locale, which will format numbers to the given style.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterCreate(
    _ allocator: CFAllocator!,
    _ locale: CFLocale!,
    _ style: CFNumberFormatterStyle
) -> CFNumberFormatter!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`locale`  

A locale to use for localization. If `NULL`, the function uses the default system locale. Use CFLocaleCopyCurrent() to specify the locale of the current user.

`style`  

A number style. See Number Formatter Styles for possible values.

## Return Value

A new number formatter, localized to the given locale, which will format numbers using the given style. Returns `NULL` if there was a problem creating the formatter. Ownership follows the The Create Rule.

