

- Core Foundation
-  CFBundleUnloadExecutable(\_:) 

Function

# CFBundleUnloadExecutable(\_:)

Unloads the main executable for the specified bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleUnloadExecutable(_ bundle: CFBundle!)
```

## Parameters 

`bundle`  

The bundle whose main executable you want to unload.

## Discussion

You should typically try to avoid using this function, but instead use CFBundleGetFunctionPointerForName(_:_:) and related functions since these make management of the bundle easier (when the last reference to the CFBundle object is released, and it is finally deallocated, then the code will be unloaded if it is still loaded, and if the executable is of a type that supports unloading).

## See Also

### Loading and Unloading a Bundle

func CFBundleIsExecutableLoaded(CFBundle!) -> Bool

Obtains information about the load status for a bundle’s main executable.

func CFBundlePreflightExecutable(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded or appears to be loadable.

func CFBundleLoadExecutable(CFBundle!) -> Bool

Loads a bundle’s main executable code into memory and dynamically links it into the running application.

func CFBundleLoadExecutableAndReturnError(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded, attempting to load it if necessary.

