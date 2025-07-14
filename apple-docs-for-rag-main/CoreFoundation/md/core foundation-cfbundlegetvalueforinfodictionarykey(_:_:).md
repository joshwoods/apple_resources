

- Core Foundation
-  CFBundleGetValueForInfoDictionaryKey(\_:\_:) 

Function

# CFBundleGetValueForInfoDictionaryKey(\_:\_:)

Returns a value (localized if possible) from a bundle’s information dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetValueForInfoDictionaryKey(
    _ bundle: CFBundle!,
    _ key: CFString!
) -> CFTypeRef!
```

## Parameters 

`bundle`  

The bundle to examine.

`key`  

The key for the value to return.

## Return Value

A value corresponding to `key` in `bundle`’s information dictionary. If available, a localized value is returned, otherwise the global value is returned. Ownership follows the The Get Rule.

## Discussion

You should use this function rather than retrieving values directly from the info dictionary (`Info.plist`) because `CFBundleGetValueForInfoDictionaryKey` returns localized values if any are available (from the `InfoPlist.strings` file for the current locale).

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

func CFBundleCopyInfoDictionaryInDirectory(CFURL!) -> CFDictionary!

Returns a bundle’s information dictionary.

func CFBundleCopyInfoDictionaryForURL(CFURL!) -> CFDictionary!

Returns the information dictionary for a given URL location.

func CFBundleGetPackageInfo(CFBundle!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutablePointer&lt;UInt32>!)

Returns a bundle’s package type and creator.

func CFBundleGetPackageInfoInDirectory(CFURL!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutablePointer&lt;UInt32>!) -> Bool

Returns a bundle’s package type and creator without having to create a CFBundle object.

func CFBundleCopyExecutableArchitectures(CFBundle!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given bundle provides.

func CFBundleCopyExecutableArchitecturesForURL(CFURL!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given URL provides.

func CFBundleGetVersionNumber(CFBundle!) -> UInt32

Returns a bundle’s version number.

