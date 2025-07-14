

- Core Foundation
-  CFBundleGetMainBundle() 

Function

# CFBundleGetMainBundle()

Returns an application’s main bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetMainBundle() -> CFBundle!
```

## Return Value

A CFBundle object representing the application’s main bundle, or `NULL` if it is not possible to create a bundle. Ownership follows the The Get Rule.

## Discussion

CFBundle creates a main bundle whenever it possibly can, even for unbundled apps. There are a few situations in which it is not possible, so you should check the return value against `NULL`, but this happens only in exceptional circumstances.

For an explanation of the main bundle, see Locating and Opening Bundles in Bundle Programming Guide.

## See Also

### Creating and Accessing Bundles

func CFBundleCreate(CFAllocator!, CFURL!) -> CFBundle!

Creates a CFBundle object.

func CFBundleCreateBundlesFromDirectory(CFAllocator!, CFURL!, CFString!) -> CFArray!

Searches a directory and constructs an array of CFBundle objects from all valid bundles in the specified directory.

func CFBundleGetAllBundles() -> CFArray!

Returns an array containing all of the bundles currently open in the application.

func CFBundleGetBundleWithIdentifier(CFString!) -> CFBundle!

Locate a bundle given its program-defined identifier.

