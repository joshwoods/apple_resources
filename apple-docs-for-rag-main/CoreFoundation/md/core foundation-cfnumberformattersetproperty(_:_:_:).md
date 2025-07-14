

- Core Foundation
-  CFNumberFormatterSetProperty(\_:\_:\_:) 

Function

# CFNumberFormatterSetProperty(\_:\_:\_:)

Sets a number formatter property using a key-value pair.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterSetProperty(
    _ formatter: CFNumberFormatter!,
    _ key: CFNumberFormatterKey!,
    _ value: CFTypeRef!
)
```

## Parameters 

`formatter`  

The number formatter to modify.

`key`  

The name of the property of `formatter` to set. See Number Formatter Property Keys for a description of possible values.

`value`  

The value of the specified key. This must be an instance of the correct `CFType` object for the corresponding key.

## See Also

### Configuring a Number Formatter

func CFNumberFormatterSetFormat(CFNumberFormatter!, CFString!)

Sets the format string of a number formatter.

