

- Core Foundation
-  CFNumberFormatterGetLocale(\_:) 

Function

# CFNumberFormatterGetLocale(\_:)

Returns the locale object used to create the given number formatter object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterGetLocale(_ formatter: CFNumberFormatter!) -> CFLocale!
```

## Parameters 

`formatter`  

The number formatter to examine.

## Return Value

The locale used to create `formatter`. Ownership follows the The Get Rule.

## See Also

### Examining a Number Formatter

func CFNumberFormatterCopyProperty(CFNumberFormatter!, CFNumberFormatterKey!) -> CFTypeRef!

Returns a copy of a number formatter’s value for a given key.

func CFNumberFormatterGetFormat(CFNumberFormatter!) -> CFString!

Returns a format string for the given number formatter object.

func CFNumberFormatterGetStyle(CFNumberFormatter!) -> CFNumberFormatterStyle

Returns the number style used to create the given number formatter object.

