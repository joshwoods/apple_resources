

- Core Foundation
-  CFBundleIsExecutableLoaded(\_:) 

Function

# CFBundleIsExecutableLoaded(\_:)

Obtains information about the load status for a bundle’s main executable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleIsExecutableLoaded(_ bundle: CFBundle!) -> Bool
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

`true` if `bundle`’s main executable has been loaded, otherwise `false`.

## See Also

### Loading and Unloading a Bundle

func CFBundlePreflightExecutable(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded or appears to be loadable.

func CFBundleLoadExecutable(CFBundle!) -> Bool

Loads a bundle’s main executable code into memory and dynamically links it into the running application.

func CFBundleLoadExecutableAndReturnError(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded, attempting to load it if necessary.

func CFBundleUnloadExecutable(CFBundle!)

Unloads the main executable for the specified bundle.

