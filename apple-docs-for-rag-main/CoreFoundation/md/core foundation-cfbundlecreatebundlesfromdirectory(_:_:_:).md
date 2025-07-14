

- Core Foundation
-  CFBundleCreateBundlesFromDirectory(\_:\_:\_:) 

Function

# CFBundleCreateBundlesFromDirectory(\_:\_:\_:)

Searches a directory and constructs an array of CFBundle objects from all valid bundles in the specified directory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCreateBundlesFromDirectory(
    _ allocator: CFAllocator!,
    _ directoryURL: CFURL!,
    _ bundleType: CFString!
) -> CFArray!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`directoryURL`  

The location of the directory to search for valid bundles.

`bundleType`  

The abstract type of the bundles to locate and create. The type is expressed as a filename extension, such as `bundle`. Pass `NULL` to create CFBundle objects for bundles of any type.

## Return Value

A CFArray object containing CFBundle objects created from the contents of the specified directory. Returns an empty array if no bundles exist at `directoryURL`, and `NULL` if there was a memory allocation problem. Ownership follows the The Create Rule.

## Discussion

The array returned by this function will not contain stale CFBundle references.

### Special Considerations

The The Create Rule applies both to the array returned and to the bundles in the array. In order to properly dispose of the returned value, you must release the array *and* any bundles returned in the array.

## See Also

### Creating and Accessing Bundles

func CFBundleCreate(CFAllocator!, CFURL!) -> CFBundle!

Creates a CFBundle object.

func CFBundleGetAllBundles() -> CFArray!

Returns an array containing all of the bundles currently open in the application.

func CFBundleGetBundleWithIdentifier(CFString!) -> CFBundle!

Locate a bundle given its program-defined identifier.

func CFBundleGetMainBundle() -> CFBundle!

Returns an application’s main bundle.

