

- Core Foundation
-  CFDateFormatterGetDateStyle(\_:) 

Function

# CFDateFormatterGetDateStyle(\_:)

Returns the date style used to create the given date formatter object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterGetDateStyle(_ formatter: CFDateFormatter!) -> CFDateFormatterStyle
```

## Parameters 

`formatter`  

The date formatter to examine.

## Return Value

The date style used to create `formatter`.

## See Also

### Getting Information About a Date Formatter

func CFDateFormatterCopyProperty(CFDateFormatter!, CFDateFormatterKey!) -> CFTypeRef!

Returns a copy of a date formatter’s value for a given key.

func CFDateFormatterGetFormat(CFDateFormatter!) -> CFString!

Returns a format string for the given date formatter object.

func CFDateFormatterGetLocale(CFDateFormatter!) -> CFLocale!

Returns the locale object used to create the given date formatter object.

func CFDateFormatterGetTimeStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the time style used to create the given date formatter object.

