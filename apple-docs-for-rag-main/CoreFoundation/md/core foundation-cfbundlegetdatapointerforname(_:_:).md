

- Core Foundation
-  CFBundleGetDataPointerForName(\_:\_:) 

Function

# CFBundleGetDataPointerForName(\_:\_:)

Returns a data pointer to a symbol of the given name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetDataPointerForName(
    _ bundle: CFBundle!,
    _ symbolName: CFString!
) -> UnsafeMutableRawPointer!
```

## Parameters 

`bundle`  

The bundle to examine.

`symbolName`  

The name of the symbol you are searching for.

## Return Value

A data pointer to a symbol named `symbolName` in `bundle`, or `NULL` if `symbolName` cannot be found. Ownership follows the The Get Rule.

## See Also

### Managing Executable Code

func CFBundleGetDataPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Returns a C array of data pointer to symbols of the given names.

func CFBundleGetFunctionPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a pointer to a function in a bundle’s executable code using the function name as the search key.

func CFBundleGetFunctionPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Constructs a function table containing pointers to all of the functions found in a bundle’s main executable code.

func CFBundleGetPlugIn(CFBundle!) -> CFPlugIn!

Returns a bundle’s plug-in.

