

- Core Foundation
-  CFStringGetDoubleValue(\_:) 

Function

# CFStringGetDoubleValue(\_:)

Returns the primary `double` value represented by a string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetDoubleValue(_ str: CFString!) -> Double
```

## Parameters 

`str`  

A string that represents a double value. The only allowed characters are the ASCII digit characters (ASCII `0x30` - `0x39`), the plus sign (ASCII `0x2B`), the minus sign (ASCII `0x2D`), and the period character (ASCII `0x2E`).

## Return Value

The `double` value represented by `str`, or `0.0` if there is a scanning error (if the string contains disallowed characters or does not represent a double value).

## Discussion

Consider the following example:

```
double val = CFStringGetDoubleValue(CFSTR("0.123"));
```

The variable `val` in this example would contain the value `0.123` after the function is called.

## See Also

### Getting Numeric Values

func CFStringGetIntValue(CFString!) -> Int32

Returns the integer value represented by a string.

