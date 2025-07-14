

- Core Foundation
-  CFBundleCopyResourceURLInDirectory(\_:\_:\_:\_:) 

Function

# CFBundleCopyResourceURLInDirectory(\_:\_:\_:\_:)

Returns the location of a resource contained in the specified bundle directory without requiring the creation of a CFBundle object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyResourceURLInDirectory(
    _ bundleURL: CFURL!,
    _ resourceName: CFString!,
    _ resourceType: CFString!,
    _ subDirName: CFString!
) -> CFURL!
```

## Parameters 

`bundleURL`  

The bundle to examine.

`resourceName`  

The name of the requested resource.

`resourceType`  

The abstract type of the requested resource. The type is expressed as a filename extension, such as `jpg`. Pass `NULL` if you don’t need to search by type.

`subDirName`  

The name of the subdirectory of the bundle’s resources directory to search. Pass `NULL` to search the standard CFBundle resource locations.

## Return Value

A CFURL object describing the location of the requested resource, or `NULL` if the resource cannot be found. Ownership follows the The Create Rule.

## Discussion

This function provides a means to obtain package information for a bundle without first creating a bundle. However, since CFBundle objects cache search results, it is faster to create a CFBundle object if you need to repeatedly access resources.

Note that searches are case-sensitive, even on file systems (such as HFS+) that are not case sensitive with regards to file names.

## See Also

### Locating Bundle Resources

func CFBundleCloseBundleResourceMap(CFBundle!, CFBundleRefNum)

Closes an open resource map for a bundle.

Deprecated

func CFBundleCopyResourceURL(CFBundle!, CFString!, CFString!, CFString!) -> CFURL!

Returns the location of a resource contained in the specified bundle.

func CFBundleCopyResourceURLsOfType(CFBundle!, CFString!, CFString!) -> CFArray!

Assembles an array of URLs specifying all of the resources of the specified type found in a bundle.

func CFBundleCopyResourceURLsOfTypeInDirectory(CFURL!, CFString!, CFString!) -> CFArray!

Returns an array of CFURL objects describing the locations of all resources in a bundle of the specified type without needing to create a CFBundle object.

func CFBundleCopyResourceURLForLocalization(CFBundle!, CFString!, CFString!, CFString!, CFString!) -> CFURL!

Returns the location of a localized resource in a bundle.

func CFBundleCopyResourceURLsOfTypeForLocalization(CFBundle!, CFString!, CFString!, CFString!) -> CFArray!

Returns an array containing copies of the URL locations for a specified bundle, resource, and localization name.

func CFBundleOpenBundleResourceFiles(CFBundle!, UnsafeMutablePointer&lt;CFBundleRefNum>!, UnsafeMutablePointer&lt;CFBundleRefNum>!) -> Int32

Opens the non-localized and localized resource files (if any) for a bundle in separate resource maps.

Deprecated

func CFBundleOpenBundleResourceMap(CFBundle!) -> CFBundleRefNum

Opens the non-localized and localized resource files (if any) for a bundle in a single resource map.

Deprecated

