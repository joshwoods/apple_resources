

- Core Foundation
-  CFBooleanGetValue(\_:) 

Function

# CFBooleanGetValue(\_:)

Returns the value of a CFBoolean object as a standard C type `Boolean`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBooleanGetValue(_ boolean: CFBoolean!) -> Bool
```

## Parameters 

`boolean`  

The boolean to examine.

## Return Value

The value of `boolean`.

## See Also

### CFBoolean Miscellaneous Functions

func CFBooleanGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for the CFBoolean opaque type.

