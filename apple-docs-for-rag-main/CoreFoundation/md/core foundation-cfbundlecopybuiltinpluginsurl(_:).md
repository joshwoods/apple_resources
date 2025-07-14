

- Core Foundation
-  CFBundleCopyBuiltInPlugInsURL(\_:) 

Function

# CFBundleCopyBuiltInPlugInsURL(\_:)

Returns the location of a bundle’s built in plug-in.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyBuiltInPlugInsURL(_ bundle: CFBundle!) -> CFURL!
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

A CFURL object describing the location of `bundle`’s built in plug-ins, or `NULL` if it could not be found. Ownership follows the The Create Rule.

## See Also

### Finding Locations in a Bundle

func CFBundleCopyAuxiliaryExecutableURL(CFBundle!, CFString!) -> CFURL!

Returns the location of a bundle’s auxiliary executable code.

func CFBundleCopyExecutableURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s main executable code.

func CFBundleCopyPrivateFrameworksURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s private Frameworks directory.

func CFBundleCopyResourcesDirectoryURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s Resources directory.

func CFBundleCopySharedFrameworksURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s shared frameworks directory.

func CFBundleCopySharedSupportURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s shared support files directory.

func CFBundleCopySupportFilesDirectoryURL(CFBundle!) -> CFURL!

Returns the location of the bundle’s support files directory.

