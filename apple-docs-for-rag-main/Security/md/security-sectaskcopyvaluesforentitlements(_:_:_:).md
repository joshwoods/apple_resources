

- Security
-  SecTaskCopyValuesForEntitlements(\_:\_:\_:) 

Function

# SecTaskCopyValuesForEntitlements(\_:\_:\_:)

Returns the values of multiple entitlements for the represented task.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTaskCopyValuesForEntitlements(
    _ task: SecTask,
    _ entitlements: CFArray,
    _ error: UnsafeMutablePointer?>?
) -> CFDictionary?
```

## Parameters 

`task`  

The task whose entitlements you want.

`entitlements`  

An array of the names of the entitlement to be fetched.

`error`  

A pointer that the function uses to provide an error object with details if an error occurs. The caller becomes responsible for the object’s memory. Pass `NULL` to ignore the error.

## Return Value

A dictionary containing the entitlement names as keys with the corresponding entitlements as the dictionary values, or `NULL` on error. In Objective-C, call the CFRelease function to free this dictionary’s memory when you are done with it.

