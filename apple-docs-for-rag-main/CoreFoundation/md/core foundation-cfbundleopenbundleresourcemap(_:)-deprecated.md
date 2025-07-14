

- Core Foundation
-  CFBundleOpenBundleResourceMap(\_:) Deprecated

Function

# CFBundleOpenBundleResourceMap(\_:)

Opens the non-localized and localized resource files (if any) for a bundle in a single resource map.

macOS 10.0–10.15Deprecated

``` source
func CFBundleOpenBundleResourceMap(_ bundle: CFBundle!) -> CFBundleRefNum
```

Deprecated

The Carbon Resource Manager is deprecated. This should only be used to access Resource Manager-style resources in old bundles.

## Parameters 

`bundle`  

The bundle whose resource map you want to open.

## Return Value

A distinct reference number for the resource map.

## Discussion

Creates and makes current a single read-only resource map containing the non-localized and localized resource files. If this function is called multiple times, it opens the files multiple times and returns distinct reference numbers for each. Use CFBundleCloseBundleResourceMap(_:_:) to close a resource map.

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

func CFBundleCopyResourceURLsOfTypeForLocalization(CFBundle!, CFString!, CFString!, CFString!) -> CFArray!

Returns an array containing copies of the URL locations for a specified bundle, resource, and localization name.

func CFBundleOpenBundleResourceFiles(CFBundle!, UnsafeMutablePointer&lt;CFBundleRefNum>!, UnsafeMutablePointer&lt;CFBundleRefNum>!) -> Int32

Opens the non-localized and localized resource files (if any) for a bundle in separate resource maps.

Deprecated

