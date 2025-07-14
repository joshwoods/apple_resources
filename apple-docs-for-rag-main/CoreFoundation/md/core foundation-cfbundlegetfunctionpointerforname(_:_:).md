

- Core Foundation
-  CFBundleGetFunctionPointerForName(\_:\_:) 

Function

# CFBundleGetFunctionPointerForName(\_:\_:)

Returns a pointer to a function in a bundle’s executable code using the function name as the search key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetFunctionPointerForName(
    _ bundle: CFBundle!,
    _ functionName: CFString!
) -> UnsafeMutableRawPointer!
```

## Parameters 

`bundle`  

The bundle to examine.

`functionName`  

The name of the function to locate.

## Return Value

A pointer to a function in a `bundle`’s executable code, or `NULL` if `functionName` cannot be found. Ownership follows the The Get Rule.

## Discussion

Calling this function will cause the bundle’s code to be loaded if necessary.

## See Also

### Managing Executable Code

func CFBundleGetDataPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a data pointer to a symbol of the given name.

func CFBundleGetDataPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Returns a C array of data pointer to symbols of the given names.

func CFBundleGetFunctionPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Constructs a function table containing pointers to all of the functions found in a bundle’s main executable code.

func CFBundleGetPlugIn(CFBundle!) -> CFPlugIn!

Returns a bundle’s plug-in.

