

- Core Foundation
-  CFBundleCopySupportFilesDirectoryURL(\_:) 

Function

# CFBundleCopySupportFilesDirectoryURL(\_:)

Returns the location of the bundle’s support files directory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopySupportFilesDirectoryURL(_ bundle: CFBundle!) -> CFURL!
```

## Parameters 

`bundle`  

The CFBundle object whose support files directory you want to locate.

## Return Value

A CFURL object describing the location of the bundle’s support files directory, or `NULL` if it could not be found. Ownership follows the The Create Rule.

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

func CFBundleCopyResourcesDirectoryURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s Resources directory.

func CFBundleCopySharedFrameworksURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s shared frameworks directory.

func CFBundleCopySharedSupportURL(CFBundle!) -> CFURL!

Returns the location of a bundle’s shared support files directory.

