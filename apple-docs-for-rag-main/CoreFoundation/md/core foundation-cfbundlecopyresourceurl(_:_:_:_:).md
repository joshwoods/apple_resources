

- Core Foundation
-  CFBundleCopyResourceURL(\_:\_:\_:\_:) 

Function

# CFBundleCopyResourceURL(\_:\_:\_:\_:)

Returns the location of a resource contained in the specified bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyResourceURL(
    _ bundle: CFBundle!,
    _ resourceName: CFString!,
    _ resourceType: CFString!,
    _ subDirName: CFString!
) -> CFURL!
```

## Parameters 

`bundle`  

The bundle to examine.

`resourceName`  

The name of the requested resource.

`resourceType`  

The abstract type of the requested resource. The type is expressed as a filename extension, such as `jpg`. Pass `NULL` if `resourceName` is the complete name of the file you’re looking for, including any extension.

`subDirName`  

The name of the subdirectory of the bundle’s resources directory to search. Pass `NULL` to search the standard CFBundle resource locations.

## Return Value

A CFURL object describing the location of the requested resource, or `NULL` if the resource cannot be found. Ownership follows the The Create Rule.

## Discussion

For example, if a bundle contains a subdirectory `WaterSounds` that includes a file `Water1.aiff`, you can retrieve the URL for the file using:

```
```

## See Also

### Locating Bundle Resources

func CFBundleCloseBundleResourceMap(CFBundle!, CFBundleRefNum)

Closes an open resource map for a bundle.

Deprecated

func CFBundleCopyResourceURLInDirectory(CFURL!, CFString!, CFString!, CFString!) -> CFURL!

Returns the location of a resource contained in the specified bundle directory without requiring the creation of a CFBundle object.

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

