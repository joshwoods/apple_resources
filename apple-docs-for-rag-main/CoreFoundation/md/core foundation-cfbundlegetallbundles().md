

- Core Foundation
-  CFBundleGetAllBundles() 

Function

# CFBundleGetAllBundles()

Returns an array containing all of the bundles currently open in the application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetAllBundles() -> CFArray!
```

## Return Value

A CFArray object containing CFBundle objects for each open bundle in the application. Ownership follows the The Get Rule.

## Discussion

This function is potentially expensive and not thread-safe. It’s best used for debugging or other diagnostics purposes rather than as part of the main execution path of production code.

## See Also

### Creating and Accessing Bundles

func CFBundleCreate(CFAllocator!, CFURL!) -> CFBundle!

Creates a CFBundle object.

func CFBundleCreateBundlesFromDirectory(CFAllocator!, CFURL!, CFString!) -> CFArray!

Searches a directory and constructs an array of CFBundle objects from all valid bundles in the specified directory.

func CFBundleGetBundleWithIdentifier(CFString!) -> CFBundle!

Locate a bundle given its program-defined identifier.

func CFBundleGetMainBundle() -> CFBundle!

Returns an application’s main bundle.

