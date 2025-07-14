

- Core Foundation
-  CFBundleGetVersionNumber(\_:) 

Function

# CFBundleGetVersionNumber(\_:)

Returns a bundle’s version number.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleGetVersionNumber(_ bundle: CFBundle!) -> UInt32
```

## Parameters 

`bundle`  

The bundle to examine. The bundle’s version number can be number or a string of the standard form “2.5.3d5”.

## Return Value

A `vers` resource style version number. If it is a string, it is automatically converted to the numeric representation, where the major version number is restricted to 2 BCD digits (in other words, it must be in the range 0-99) and the minor and bug fix version numbers are each restricted to a single BCD digit (0-9).

## Discussion

This function is only supported for the `vers` resource style version numbers. Where other version number styles—namely X, or X.Y, or X.Y.Z—are used, you can use CFBundleGetValueForInfoDictionaryKey(_:_:) with the key `kCFBundleVersionKey` to extract the version number as a string from the bundle’s information dictionary.

Some version numbers of the form X, X.Y, and X.Y.Z may work with this function, if X \

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

func CFBundleGetPackageInfoInDirectory(CFURL!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutablePointer&lt;UInt32>!) -> Bool

Returns a bundle’s package type and creator without having to create a CFBundle object.

func CFBundleCopyExecutableArchitectures(CFBundle!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given bundle provides.

func CFBundleCopyExecutableArchitecturesForURL(CFURL!) -> CFArray!

Returns an array of CFNumbers representing the architectures a given URL provides.

