

- Core Foundation
-  CFBundleOpenBundleResourceFiles(\_:\_:\_:) Deprecated

Function

# CFBundleOpenBundleResourceFiles(\_:\_:\_:)

Opens the non-localized and localized resource files (if any) for a bundle in separate resource maps.

macOS 10.0–10.15Deprecated

``` source
func CFBundleOpenBundleResourceFiles(
    _ bundle: CFBundle!,
    _ refNum: UnsafeMutablePointer!,
    _ localizedRefNum: UnsafeMutablePointer!
) -> Int32
```

Deprecated

The Carbon Resource Manager is deprecated. This should only be used to access Resource Manager-style resources in old bundles.

## Parameters 

`bundle`  

The bundle whose resource map you want to open.

`refNum`  

On return, the reference number of the non-localized resource map.

`localizedRefNum`  

On return, the reference number of the localized resource map.

## Return Value

An error code. The function returns `0` (`noErr`) if successful. If the bundle contains more than one resource file, the function returns an error code only if none was opened. The most common error is `resFNotFound`, but the function may also pass through other errors returned from the Resource Manager.

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

func CFBundleOpenBundleResourceMap(CFBundle!) -> CFBundleRefNum

Opens the non-localized and localized resource files (if any) for a bundle in a single resource map.

Deprecated

