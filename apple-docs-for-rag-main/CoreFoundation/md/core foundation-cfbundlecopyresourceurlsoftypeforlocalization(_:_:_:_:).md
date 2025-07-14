

- Core Foundation
-  CFBundleCopyResourceURLsOfTypeForLocalization(\_:\_:\_:\_:) 

Function

# CFBundleCopyResourceURLsOfTypeForLocalization(\_:\_:\_:\_:)

Returns an array containing copies of the URL locations for a specified bundle, resource, and localization name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyResourceURLsOfTypeForLocalization(
    _ bundle: CFBundle!,
    _ resourceType: CFString!,
    _ subDirName: CFString!,
    _ localizationName: CFString!
) -> CFArray!
```

## Parameters 

`bundle`  

The bundle to examine.

`resourceType`  

The abstract type of the resources to locate. The type is expressed as a filename extension, such as `jpg`.

`subDirName`  

The name of the subdirectory of the bundle’s Resources directory to search. Pass `NULL` to search the standard CFBundle resource locations.

`localizationName`  

The name of the localization. This value should correspond to the name of one of the bundle’s language-specific resource directories without the `.lproj` extension. (This parameter is treated literally: If you pass `"de"`, the function will not match resources in a `German.lproj` directory in the bundle.)

## Return Value

A CFArray object containing copies of the requested locations. Ownership follows the The Create Rule.

## Discussion

Note that file names are case-sensitive, even on file systems (such as HFS+) that are not case sensitive with regards to file names.

You should typically have little reason to use this function (see Getting the Current Language and Locale)—CFBundle’s interfaces automatically apply the user’s preferences to determine which localized resource files to return in response to a programmatic request. See also CFBundleCopyBundleLocalizations(_:) for how to determine what localizations are available

## See Also

### Locating Bundle Resources

func CFBundleCloseBundleResourceMap(CFBundle!, CFBundleRefNum)

Closes an open resource map for a bundle.

Deprecated

func CFBundleCopyResourceURL(CFBundle!, CFString!, CFString!, CFString!) -> CFURL!

Returns the location of a resource contained in the specified bundle.

func CFBundleCopyResourceURLInDirectory(CFURL!, CFString!, CFString!, CFString!) -> CFURL!

Returns the location of a resource contained in the specified bundle directory without requiring the creation of a CFBundle object.

func CFBundleCopyResourceURLsOfType(CFBundle!, CFString!, CFString!) -> CFArray!

Assembles an array of URLs specifying all of the resources of the specified type found in a bundle.

func CFBundleCopyResourceURLsOfTypeInDirectory(CFURL!, CFString!, CFString!) -> CFArray!

Returns an array of CFURL objects describing the locations of all resources in a bundle of the specified type without needing to create a CFBundle object.

func CFBundleCopyResourceURLForLocalization(CFBundle!, CFString!, CFString!, CFString!, CFString!) -> CFURL!

Returns the location of a localized resource in a bundle.

func CFBundleOpenBundleResourceFiles(CFBundle!, UnsafeMutablePointer&lt;CFBundleRefNum>!, UnsafeMutablePointer&lt;CFBundleRefNum>!) -> Int32

Opens the non-localized and localized resource files (if any) for a bundle in separate resource maps.

Deprecated

func CFBundleOpenBundleResourceMap(CFBundle!) -> CFBundleRefNum

Opens the non-localized and localized resource files (if any) for a bundle in a single resource map.

Deprecated

