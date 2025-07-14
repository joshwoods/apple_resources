

- Core Foundation
-  CFDateFormatterGetFormat(\_:) 

Function

# CFDateFormatterGetFormat(\_:)

Returns a format string for the given date formatter object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterGetFormat(_ formatter: CFDateFormatter!) -> CFString!
```

## Parameters 

`formatter`  

The date formatter to examine.

## Return Value

The format string for `formatter` as was specified by calling the CFDateFormatterSetFormat(_:_:) function, or derived from the date formatter’s date or time styles. Ownership follows the The Get Rule.

## See Also

### Getting Information About a Date Formatter

func CFDateFormatterCopyProperty(CFDateFormatter!, CFDateFormatterKey!) -> CFTypeRef!

Returns a copy of a date formatter’s value for a given key.

func CFDateFormatterGetDateStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the date style used to create the given date formatter object.

func CFDateFormatterGetLocale(CFDateFormatter!) -> CFLocale!

Returns the locale object used to create the given date formatter object.

func CFDateFormatterGetTimeStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the time style used to create the given date formatter object.

