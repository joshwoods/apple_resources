

- Core Foundation
-  CFBundleCopyAuxiliaryExecutableURL(\_:\_:) 

Function

# CFBundleCopyAuxiliaryExecutableURL(\_:\_:)

Returns the location of a bundle’s auxiliary executable code.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyAuxiliaryExecutableURL(
    _ bundle: CFBundle!,
    _ executableName: CFString!
) -> CFURL!
```

## Parameters 

`bundle`  

The bundle to examine.

`executableName`  

The name of `bundle`’s auxiliary executable code.

## Return Value

The URL location of the specified bundle’s auxiliary executable code, or `NULL` if it could not be found. Ownership follows the The Create Rule.

## Discussion

This function can be used to find executables other than your main executable. This is useful, for instance, for applications that have some command line tool that is packaged with and used by the application. The tool can be packaged in the various platform executable directories in the bundle and can be located with this function. This allows an application to ship versions of the tool for each platform as it does for the main application executable.

## See Also

### Finding Locations in a Bundle

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

func CFBundleCopySupportFilesDirectoryURL(CFBundle!) -> CFURL!

Returns the location of the bundle’s support files directory.

