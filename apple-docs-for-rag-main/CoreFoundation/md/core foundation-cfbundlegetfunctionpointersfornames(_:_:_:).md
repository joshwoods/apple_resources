

- Core Foundation
-  CFBundleGetFunctionPointersForNames(\_:\_:\_:) 

Function

# CFBundleGetFunctionPointersForNames(\_:\_:\_:)

Constructs a function table containing pointers to all of the functions found in a bundle’s main executable code.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetFunctionPointersForNames(
    _ bundle: CFBundle!,
    _ functionNames: CFArray!,
    _ ftbl: UnsafeMutablePointer!
)
```

## Parameters 

`bundle`  

The bundle to examine.

`functionNames`  

A CFArray object containing a list of the function names to locate.

`ftbl`  

A C array into which this function stores the function pointers for the symbols specified in `functionNames`. The array contains `NULL` for any names in `functionNames` that cannot be found.

## Discussion

Calling this function causes the bundle’s code to be loaded if necessary.

## See Also

### Managing Executable Code

func CFBundleGetDataPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a data pointer to a symbol of the given name.

func CFBundleGetDataPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Returns a C array of data pointer to symbols of the given names.

func CFBundleGetFunctionPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a pointer to a function in a bundle’s executable code using the function name as the search key.

func CFBundleGetPlugIn(CFBundle!) -> CFPlugIn!

Returns a bundle’s plug-in.

