

- Core Foundation
-  CFBundleGetPlugIn(\_:) 

Function

# CFBundleGetPlugIn(\_:)

Returns a bundle’s plug-in.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetPlugIn(_ bundle: CFBundle!) -> CFPlugIn!
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

The plug-in for `bundle`. Ownership follows the The Get Rule.

## See Also

### Managing Executable Code

func CFBundleGetDataPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a data pointer to a symbol of the given name.

func CFBundleGetDataPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Returns a C array of data pointer to symbols of the given names.

func CFBundleGetFunctionPointerForName(CFBundle!, CFString!) -> UnsafeMutableRawPointer!

Returns a pointer to a function in a bundle’s executable code using the function name as the search key.

func CFBundleGetFunctionPointersForNames(CFBundle!, CFArray!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!)

Constructs a function table containing pointers to all of the functions found in a bundle’s main executable code.

