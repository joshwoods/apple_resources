

- Core Foundation
-  CFNumberFormatterGetFormat(\_:) 

Function

# CFNumberFormatterGetFormat(\_:)

Returns a format string for the given number formatter object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterGetFormat(_ formatter: CFNumberFormatter!) -> CFString!
```

## Parameters 

`formatter`  

The number formatter to examine.

## Return Value

The format string for `formatter` as was specified by calling the CFNumberFormatterSetFormat(_:_:) function, or derived from the number formatter’s style. See Creating and Using CFNumberFormatter Objects for more information. Ownership follows the The Get Rule.

## See Also

### Examining a Number Formatter

func CFNumberFormatterCopyProperty(CFNumberFormatter!, CFNumberFormatterKey!) -> CFTypeRef!

Returns a copy of a number formatter’s value for a given key.

func CFNumberFormatterGetLocale(CFNumberFormatter!) -> CFLocale!

Returns the locale object used to create the given number formatter object.

func CFNumberFormatterGetStyle(CFNumberFormatter!) -> CFNumberFormatterStyle

Returns the number style used to create the given number formatter object.

