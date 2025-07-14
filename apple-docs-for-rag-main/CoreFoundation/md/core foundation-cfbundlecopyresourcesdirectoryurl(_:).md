

- Core Foundation
-  CFBundleCopyResourcesDirectoryURL(\_:) 

Function

# CFBundleCopyResourcesDirectoryURL(\_:)

Returns the location of a bundle’s Resources directory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyResourcesDirectoryURL(_ bundle: CFBundle!) -> CFURL!
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

A CFURL object describing the location of `bundle`’s resources directory, or `NULL` if it could not be found. Ownership follows the The Create Rule.

## Discussion

In general, you should never need to use this function. Use CFBundleCopyResourceURL(_:_:_:_:) and similar functions instead.

## See Also

### Finding Locations in a Bundle

func CFBundleCopyAuxiliaryExecutableURL(CFBundle!, CFString!) -> CFURL!

Returns the location of a bundle’s auxiliary executable code.

func CFBundleCopyBuiltInPlugInsURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s built in plug-in.

func CFBundleCopyExecutableURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s main executable code.

func CFBundleCopyPrivateFrameworksURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s private Frameworks directory.

func CFBundleCopySharedFrameworksURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s shared frameworks directory.

func CFBundleCopySharedSupportURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s shared support files directory.

func CFBundleCopySupportFilesDirectoryURL(CFBundle!) -> CFURL!

Returns the location of the bundle’s support files directory.

