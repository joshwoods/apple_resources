

- Core Foundation
-  CFBundleGetDevelopmentRegion(\_:) 

Function

# CFBundleGetDevelopmentRegion(\_:)

Returns the bundle’s development region from the bundle’s information property list.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetDevelopmentRegion(_ bundle: CFBundle!) -> CFString!
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

A CFString object containing the name of the bundle’s development region. Ownership follows the The Get Rule.

## See Also

### Getting Bundle Properties

func CFBundleCopyBundleURL(CFBundle!) -> CFURL!

Returns the location of a bundle.

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

