

- Core Foundation
-  CFBundleCopyBundleURL(\_:) 

Function

# CFBundleCopyBundleURL(\_:)

Returns the location of a bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyBundleURL(_ bundle: CFBundle!) -> CFURL!
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

A CFURL object describing the location of `bundle`, or `NULL` if the specified bundle does not exist. Ownership follows the The Create Rule.

## See Also

### Getting Bundle Properties

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

func CFBundleGetPackageInfoInDirectory(CFURL!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutablePointer&lt;UInt32>!) -> Bool

Returns a bundle’s package type and creator without having to create a CFBundle object.

func CFBundleCopyExecutableArchitectures(CFBundle!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given bundle provides.

func CFBundleCopyExecutableArchitecturesForURL(CFURL!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given URL provides.

func CFBundleGetVersionNumber(CFBundle!) -> UInt32

Returns a bundle’s version number.

