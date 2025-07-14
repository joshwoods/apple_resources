

- Core Foundation
-  CFNumberFormatterGetStyle(\_:) 

Function

# CFNumberFormatterGetStyle(\_:)

Returns the number style used to create the given number formatter object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterGetStyle(_ formatter: CFNumberFormatter!) -> CFNumberFormatterStyle
```

## Parameters 

`formatter`  

The number formatter to examine.

## Return Value

The number style used to create `formatter`.

## See Also

### Examining a Number Formatter

func CFNumberFormatterCopyProperty(CFNumberFormatter!, CFNumberFormatterKey!) -> CFTypeRef!

Returns a copy of a number formatter’s value for a given key.

func CFNumberFormatterGetFormat(CFNumberFormatter!) -> CFString!

Returns a format string for the given number formatter object.

func CFNumberFormatterGetLocale(CFNumberFormatter!) -> CFLocale!

Returns the locale object used to create the given number formatter object.

