

- Application Services
- Core Printing
-  PMRelease(\_:) 

Function

# PMRelease(\_:)

Releases a printing object by decrementing its reference count.

macOS 10.0+

``` source
func PMRelease(_ object: PMObject?) -> OSStatus
```

## Parameters 

`object`  

The printing object you want to release.

## Return Value

A result code. See Result Codes.

## Discussion

Your application should use the `PMRelease` function to release any printing objects it creates or retains. When an object’s reference count reaches 0, the object is deallocated.

For example, to terminate a printing session created with the function PMCreateSession(_:), pass the associated PMPrintSession object to `PMRelease`. To release printing objects created with the functions PMCreatePageFormat(_:) and PMCreatePrintSettings(_:), pass the associated `PMPageFormat` and `PMPrintSettings` objects to `PMRelease`.

## See Also

### Releasing and Retaining Printing Objects

func PMRetain(PMObject?) -> OSStatus

Retains a printing object by incrementing its reference count.

