

- Core Foundation
-  CFBundleGetDataPointersForNames(\_:\_:\_:) 

Function

# CFBundleGetDataPointersForNames(\_:\_:\_:)

Returns a C array of data pointer to symbols of the given names.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetDataPointersForNames(
    _ bundle: CFBundle!,
    _ symbolNames: CFArray!,
    _ stbl: UnsafeMutablePointer!
)
```

## Parameters 

`bundle`  

The bundle to examine.

`symbolNames`  

A CFArray object containing CFString objects representing the symbol names to search for.

`stbl`  

A C array into which this function stores the data pointers for the symbols specified in `symbolNames`. The array contains `NULL` for any names in `symbolNames` that cannot be found.

## See Also

### Managing Executable Code

func CFBundleGetDataPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a data pointer to a symbol of the given name.

func CFBundleGetFunctionPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a pointer to a function in a bundle’s executable code using the function name as the search key.

func CFBundleGetFunctionPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Constructs a function table containing pointers to all of the functions found in a bundle’s main executable code.

func CFBundleGetPlugIn(CFBundle!) -> CFPlugIn!

Returns a bundle’s plug-in.

