

- Core Foundation
-  CFBundleCloseBundleResourceMap(\_:\_:) Deprecated

Function

# CFBundleCloseBundleResourceMap(\_:\_:)

Closes an open resource map for a bundle.

macOS 10.0–10.15Deprecated

``` source
func CFBundleCloseBundleResourceMap(
    _ bundle: CFBundle!,
    _ refNum: CFBundleRefNum
)
```

Deprecated

The Carbon Resource Manager is deprecated. This should only be used to access Resource Manager-style resources in old bundles.

## Parameters 

`bundle`  

The bundle whose resource map is referenced by `refNum`.

`refNum`  

The reference number for a resource map to close.

## Discussion

You open a resource map using either CFBundleOpenBundleResourceFiles(_:_:_:) or CFBundleOpenBundleResourceMap(_:).

## See Also

### Locating Bundle Resources

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

func CFBundleCopyResourceURLsOfTypeForLocalization(CFBundle!, CFString!, CFString!, CFString!) -> CFArray!

Returns an array containing copies of the URL locations for a specified bundle, resource, and localization name.

func CFBundleOpenBundleResourceFiles(CFBundle!, UnsafeMutablePointer&lt;CFBundleRefNum>!, UnsafeMutablePointer&lt;CFBundleRefNum>!) -> Int32

Opens the non-localized and localized resource files (if any) for a bundle in separate resource maps.

Deprecated

func CFBundleOpenBundleResourceMap(CFBundle!) -> CFBundleRefNum

Opens the non-localized and localized resource files (if any) for a bundle in a single resource map.

Deprecated

