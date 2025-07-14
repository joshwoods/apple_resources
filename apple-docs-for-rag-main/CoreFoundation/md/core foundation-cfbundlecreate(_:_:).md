

- Core Foundation
-  CFBundleCreate(\_:\_:) 

Function

# CFBundleCreate(\_:\_:)

Creates a CFBundle object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCreate(
    _ allocator: CFAllocator!,
    _ bundleURL: CFURL!
) -> CFBundle!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bundleURL`  

The location of the bundle for which to create a CFBundle object.

## Return Value

A CFBundle object created from the bundle at `bundleURL`. Ownership follows the The Create Rule.

## Discussion

Returns `NULL` if there was a memory allocation problem. May return an existing CFBundle object with the reference count incremented. May return `NULL` if the bundle doesn’t exist at `bundleURL` (see Discussion).

## Discussion

Once a bundle has been created, it is cached; the bundle cache is flushed only periodically. `CFBundleCreate` does not check that a cached bundle still exists in the filesystem. If a bundle is deleted from the filesystem, it is therefore possible for `CFBundleCreate` to return a cached bundle that has actually been deleted.

## See Also

### Creating and Accessing Bundles

func CFBundleCreateBundlesFromDirectory(CFAllocator!, CFURL!, CFString!) -> CFArray!

Searches a directory and constructs an array of CFBundle objects from all valid bundles in the specified directory.

func CFBundleGetAllBundles() -> CFArray!

Returns an array containing all of the bundles currently open in the application.

func CFBundleGetBundleWithIdentifier(CFString!) -> CFBundle!

Locate a bundle given its program-defined identifier.

func CFBundleGetMainBundle() -> CFBundle!

Returns an application’s main bundle.

