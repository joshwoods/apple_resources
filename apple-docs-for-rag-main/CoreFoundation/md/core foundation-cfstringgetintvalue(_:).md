

- Core Foundation
-  CFStringGetIntValue(\_:) 

Function

# CFStringGetIntValue(\_:)

Returns the integer value represented by a string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetIntValue(_ str: CFString!) -> Int32
```

## Parameters 

`str`  

A string that represents a signed integer value. The only allowed characters are the ASCII digit characters (ASCII `0x30` - `0x39`), the plus sign (ASCII `0x2B`), the minus sign (ASCII `0x2D`), and the period character (ASCII `0x2E`).

## Return Value

The signed integer value represented by `str`. The result is `0` if there is a scanning error (if the string contains disallowed characters or does not represent an integer value) or `INT_MAX` or `INT_MIN` if there is an overflow error.

## Discussion

Consider the following example:

```
SInt32 val = CFStringGetIntValue(CFSTR("-123"));
```

The variable `val` in this example would contain the value `-123` after the function is called.

## See Also

### Getting Numeric Values

func CFStringGetDoubleValue(CFString!) -> Double

Returns the primary `double` value represented by a string.

