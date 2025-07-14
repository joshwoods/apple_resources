

- Core Foundation
-  CFBundleCopyInfoDictionaryForURL(\_:) 

Function

# CFBundleCopyInfoDictionaryForURL(\_:)

Returns the information dictionary for a given URL location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyInfoDictionaryForURL(_ url: CFURL!) -> CFDictionary!
```

## Parameters 

`url`  

A CFURL object describing the location of a file.

## Return Value

A CFDictionary object containing `url`’s information dictionary. Ownership follows the The Create Rule.

## Discussion

For a directory URL, this is equivalent to CFBundleCopyInfoDictionaryInDirectory(_:). For a plain file URL representing an unbundled application, this function will attempt to read an information dictionary either from the `(__TEXT, __info_plist)` section of the file (for a Mach-O file) or from a `plst` resource.

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

