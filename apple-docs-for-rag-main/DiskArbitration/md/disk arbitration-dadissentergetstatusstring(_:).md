

- Disk Arbitration
-  DADissenterGetStatusString(\_:) 

Function

# DADissenterGetStatusString(\_:)

Obtains the return code string.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADissenterGetStatusString(_ dissenter: DADissenter) -> CFString?
```

## Parameters 

`dissenter`  

The DADissenter for which to obtain the return code string.

## Return Value

The return code string.

## See Also

### Miscellaneous

func DADissenterCreate(CFAllocator?, DAReturn, CFString?) -> DADissenter

Creates a new dissenter object.

func DADissenterGetStatus(DADissenter) -> DAReturn

Obtains the return code.

