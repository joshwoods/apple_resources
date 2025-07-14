

- Core Foundation
-  CFDateFormatterSetProperty(\_:\_:\_:) 

Function

# CFDateFormatterSetProperty(\_:\_:\_:)

Sets a date formatter property using a key-value pair.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterSetProperty(
    _ formatter: CFDateFormatter!,
    _ key: CFString!,
    _ value: CFTypeRef!
)
```

## Parameters 

`formatter`  

The date formatter to modify.

`key`  

The name of the property to set. See Date Formatter Property Keys for a description of possible values for this parameter.

`value`  

The value for `key`. This should be a CFType object corresponding to the specified key.

## See Also

### Configuring a Date Formatter

func CFDateFormatterSetFormat(CFDateFormatter!, CFString!)

Sets the format string of the given date formatter to the specified value.

