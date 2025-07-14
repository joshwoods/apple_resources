

- Core Foundation
-  CFBundleLoadExecutable(\_:) 

Function

# CFBundleLoadExecutable(\_:)

Loads a bundle’s main executable code into memory and dynamically links it into the running application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleLoadExecutable(_ bundle: CFBundle!) -> Bool
```

## Parameters 

`bundle`  

The bundle whose main executable you want to load.

## Return Value

`true` if the executable was successfully loaded, otherwise `false`.

## Discussion

You should typically try to avoid using this function, but instead use CFBundleGetFunctionPointerForName(_:_:) and related functions since these make memory management of the bundle easier.

## See Also

### Loading and Unloading a Bundle

func CFBundleIsExecutableLoaded(CFBundle!) -> Bool

Obtains information about the load status for a bundle’s main executable.

func CFBundlePreflightExecutable(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded or appears to be loadable.

func CFBundleLoadExecutableAndReturnError(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded, attempting to load it if necessary.

func CFBundleUnloadExecutable(CFBundle!)

Unloads the main executable for the specified bundle.

