

- Core Foundation
-  CFNumberFormatterSetFormat(\_:\_:) 

Function

# CFNumberFormatterSetFormat(\_:\_:)

Sets the format string of a number formatter.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterSetFormat(
    _ formatter: CFNumberFormatter!,
    _ formatString: CFString!
)
```

## Parameters 

`formatter`  

The number formatter to modify.

`formatString`  

The format string to be used by `formatter`. See Creating and Using CFNumberFormatter Objects for more information.

## Discussion

The format string may override other properties previously set using other functions. If this function is not called, the default value of the format string is derived from the number formatter’s style.

## See Also

### Configuring a Number Formatter

func CFNumberFormatterSetProperty(CFNumberFormatter!, CFNumberFormatterKey!, CFTypeRef!)

Sets a number formatter property using a key-value pair.

