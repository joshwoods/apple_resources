

- Disk Arbitration
-  DADissenterCreate(\_:\_:\_:) 

Function

# DADissenterCreate(\_:\_:\_:)

Creates a new dissenter object.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADissenterCreate(
    _ allocator: CFAllocator?,
    _ status: DAReturn,
    _ string: CFString?
) -> DADissenter
```

## Parameters 

`allocator`  

The allocator object to be used to allocate memory.

`status`  

The return code.

`string`  

The return code string. Pass NULL for no reason.

## Return Value

A reference to a new DADissenter.

## See Also

### Miscellaneous

func DADissenterGetStatus(DADissenter) -> DAReturn

Obtains the return code.

func DADissenterGetStatusString(DADissenter) -> CFString?

Obtains the return code string.

