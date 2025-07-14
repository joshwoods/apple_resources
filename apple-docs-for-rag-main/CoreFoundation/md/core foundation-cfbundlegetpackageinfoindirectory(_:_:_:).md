

- Core Foundation
-  CFBundleGetPackageInfoInDirectory(\_:\_:\_:) 

Function

# CFBundleGetPackageInfoInDirectory(\_:\_:\_:)

Returns a bundle’s package type and creator without having to create a CFBundle object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetPackageInfoInDirectory(
    _ url: CFURL!,
    _ packageType: UnsafeMutablePointer!,
    _ packageCreator: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`url`  

The location of a bundle.

`packageType`  

On return, the four-letter type code for the bundle. This is `APPL` for applications, `FMWK` for frameworks, and `BNDL` for generic bundles. Or a more specific type code for generic bundles.

`packageCreator`  

On return, the four-letter “creator” code for the bundle.

## Return Value

`true` if the package type and creator were found, otherwise `false`.

## See Also

### Getting Bundle Properties

func CFBundleCopyBundleURL(CFBundle!) -> CFURL!

Returns the location of a bundle.

func CFBundleGetDevelopmentRegion(CFBundle!) -> CFString!

Returns the bundle’s development region from the bundle’s information property list.

func CFBundleGetIdentifier(CFBundle!) -> CFString!

Returns the bundle identifier from a bundle’s information property list.

func CFBundleGetInfoDictionary(CFBundle!) -> CFDictionary!

Returns a bundle’s information dictionary.

func CFBundleGetLocalInfoDictionary(CFBundle!) -> CFDictionary!

Returns a bundle’s localized information dictionary.

func CFBundleGetValueForInfoDictionaryKey(CFBundle!, CFString!) -> CFTypeRef!

Returns a value (localized if possible) from a bundle’s information dictionary.

func CFBundleCopyInfoDictionaryInDirectory(CFURL!) -> CFDictionary!

Returns a bundle’s information dictionary.

func CFBundleCopyInfoDictionaryForURL(CFURL!) -> CFDictionary!

Returns the information dictionary for a given URL location.

func CFBundleGetPackageInfo(CFBundle!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutablePointer&lt;UInt32>!)

Returns a bundle’s package type and creator.

func CFBundleCopyExecutableArchitectures(CFBundle!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given bundle provides.

func CFBundleCopyExecutableArchitecturesForURL(CFURL!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given URL provides.

func CFBundleGetVersionNumber(CFBundle!) -> UInt32

Returns a bundle’s version number.

