

- Disk Arbitration
-  DADissenterGetStatus(\_:) 

Function

# DADissenterGetStatus(\_:)

Obtains the return code.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADissenterGetStatus(_ dissenter: DADissenter) -> DAReturn
```

## Parameters 

`dissenter`  

The DADissenter for which to obtain the return code.

## Return Value

The return code. A BSD return code, if applicable, is encoded with unix_err().

## See Also

### Miscellaneous

func DADissenterCreate(CFAllocator?, DAReturn, CFString?) -> DADissenter

Creates a new dissenter object.

func DADissenterGetStatusString(DADissenter) -> CFString?

Obtains the return code string.

