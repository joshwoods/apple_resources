

- Core Foundation
-  CFNumberFormatterCopyProperty(\_:\_:) 

Function

# CFNumberFormatterCopyProperty(\_:\_:)

Returns a copy of a number formatter’s value for a given key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterCopyProperty(
    _ formatter: CFNumberFormatter!,
    _ key: CFNumberFormatterKey!
) -> CFTypeRef!
```

## Parameters 

`formatter`  

The number formatter to examine.

`key`  

A property key. See Number Formatter Property Keys for valid values.

## Return Value

A `CFType` object that is a copy of the property value for `key`. Returns `NULL` if there is no value specified for `key`. Ownership follows the The Create Rule.

## See Also

### Examining a Number Formatter

func CFNumberFormatterGetFormat(CFNumberFormatter!) -> CFString!

Returns a format string for the given number formatter object.

func CFNumberFormatterGetLocale(CFNumberFormatter!) -> CFLocale!

Returns the locale object used to create the given number formatter object.

func CFNumberFormatterGetStyle(CFNumberFormatter!) -> CFNumberFormatterStyle

Returns the number style used to create the given number formatter object.

