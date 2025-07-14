

- Core Foundation
-  CFDateFormatterCopyProperty(\_:\_:) 

Function

# CFDateFormatterCopyProperty(\_:\_:)

Returns a copy of a date formatter’s value for a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterCopyProperty(
    _ formatter: CFDateFormatter!,
    _ key: CFDateFormatterKey!
) -> CFTypeRef!
```

## Parameters 

`formatter`  

The date formatter to examine.

`key`  

The property key for the value to obtain. See Date Formatter Property Keys for a description of possible values for this parameter.

## Return Value

A CFType object that is a copy of the property value for `key`, or `NULL` if there is no value specified for `key`. Ownership follows the The Create Rule.

## See Also

### Getting Information About a Date Formatter

func CFDateFormatterGetDateStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the date style used to create the given date formatter object.

func CFDateFormatterGetFormat(CFDateFormatter!) -> CFString!

Returns a format string for the given date formatter object.

func CFDateFormatterGetLocale(CFDateFormatter!) -> CFLocale!

Returns the locale object used to create the given date formatter object.

func CFDateFormatterGetTimeStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the time style used to create the given date formatter object.

