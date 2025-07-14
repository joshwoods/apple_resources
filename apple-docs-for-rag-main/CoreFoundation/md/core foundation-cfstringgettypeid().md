

- Core Foundation
-  CFStringGetTypeID() 

Function

# CFStringGetTypeID()

Returns the type identifier for the CFString opaque type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetTypeID() -> CFTypeID
```

## Return Value

The type identifier for the CFString opaque type.

## Discussion

CFMutableString objects have the same type identifier as CFString objects.

## See Also

### Getting String Properties

func CFShowStr(CFString!)

Prints the attributes of a string during debugging.

