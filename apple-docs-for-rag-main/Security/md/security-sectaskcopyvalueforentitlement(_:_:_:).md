

- Security
-  SecTaskCopyValueForEntitlement(\_:\_:\_:) 

Function

# SecTaskCopyValueForEntitlement(\_:\_:\_:)

Returns the value of a single entitlement for the represented task.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTaskCopyValueForEntitlement(
    _ task: SecTask,
    _ entitlement: CFString,
    _ error: UnsafeMutablePointer?>?
) -> CFTypeRef?
```

## Parameters 

`task`  

The task whose entitlement you want.

`entitlement`  

The name of the entitlement to be fetched.

`error`  

A pointer that the function uses to provide an error object with details if an error occurs. The caller becomes responsible for the object’s memory. Pass `NULL` to ignore the error.

## Return Value

The value of the specified entitlement for the process or `NULL` if the entitlement value could not be retrieved. The type of the returned value depends on the entitlement specified. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

## Discussion

An empty return value may indicate an error, or it may indicate that the entitlement is simply not present. In the latter case, no error is returned.

