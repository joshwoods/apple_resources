

- Core Foundation
-  CFDateFormatterGetLocale(\_:) 

Function

# CFDateFormatterGetLocale(\_:)

Returns the locale object used to create the given date formatter object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterGetLocale(_ formatter: CFDateFormatter!) -> CFLocale!
```

## Parameters 

`formatter`  

The date formatter object to examine.

## Return Value

The locale object used to create `formatter`. Ownership follows the The Get Rule.

## See Also

### Getting Information About a Date Formatter

func CFDateFormatterCopyProperty(CFDateFormatter!, CFDateFormatterKey!) -> CFTypeRef!

Returns a copy of a date formatter’s value for a given key.

func CFDateFormatterGetDateStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the date style used to create the given date formatter object.

func CFDateFormatterGetFormat(CFDateFormatter!) -> CFString!

Returns a format string for the given date formatter object.

func CFDateFormatterGetTimeStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the time style used to create the given date formatter object.

