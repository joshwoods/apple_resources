

- Core Foundation
-  CFBundleGetBundleWithIdentifier(\_:) 

Function

# CFBundleGetBundleWithIdentifier(\_:)

Locate a bundle given its program-defined identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetBundleWithIdentifier(_ bundleID: CFString!) -> CFBundle!
```

## Parameters 

`bundleID`  

The identifier of the bundle to locate. Note that identifier names are case-sensitive.

## Return Value

A CFBundle object, or `NULL` if the bundle was not found. Ownership follows the The Get Rule.

## Discussion

For a bundle to be located using its identifier, the bundle must already have been loaded. The principal purpose for locating bundles by identifier is for code in frameworks or plugins to find its own bundle.

Bundle identifiers are created by entering a value for the key `CFBundleIdentifier` in the bundle’s `Info.plist` file.

To ensure uniqueness, you should create bundle identifiers with the form of reverse-DNS naming style package names, such as `com.MyCompany.MyApp.bundleName`.

### Special Considerations

If a bundle object is created and the bundle file structure later deleted from the filesystem, this function will still return the original bundle object.

## See Also

### Creating and Accessing Bundles

func CFBundleCreate(CFAllocator!, CFURL!) -> CFBundle!

Creates a CFBundle object.

func CFBundleCreateBundlesFromDirectory(CFAllocator!, CFURL!, CFString!) -> CFArray!

Searches a directory and constructs an array of CFBundle objects from all valid bundles in the specified directory.

func CFBundleGetAllBundles() -> CFArray!

Returns an array containing all of the bundles currently open in the application.

func CFBundleGetMainBundle() -> CFBundle!

Returns an application’s main bundle.

