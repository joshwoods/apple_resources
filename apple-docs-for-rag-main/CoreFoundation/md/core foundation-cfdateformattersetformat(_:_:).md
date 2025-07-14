

- Core Foundation
-  CFDateFormatterSetFormat(\_:\_:) 

Function

# CFDateFormatterSetFormat(\_:\_:)

Sets the format string of the given date formatter to the specified value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterSetFormat(
    _ formatter: CFDateFormatter!,
    _ formatString: CFString!
)
```

## Parameters 

`formatter`  

The date formatter to modify.

`formatString`  

The format string for `formatter`. The syntax of this string is defined by Unicode Technical Standard #35..

## Discussion

The format string may override other properties previously set using other functions. If this function is not called, the default value of the format string is derived from the date formatter’s date and time styles.

## See Also

### Configuring a Date Formatter

func CFDateFormatterSetProperty(CFDateFormatter!, CFString!, CFTypeRef!)

Sets a date formatter property using a key-value pair.

