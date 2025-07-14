

- Core Foundation
-  CFBundleLoadExecutableAndReturnError(\_:\_:) 

Function

# CFBundleLoadExecutableAndReturnError(\_:\_:)

Returns a Boolean value that indicates whether a given bundle is loaded, attempting to load it if necessary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFBundleLoadExecutableAndReturnError(
    _ bundle: CFBundle!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`bundle`  

The bundle to examine.

`error`  

Upon return, if an error occurs contains a CFError that describes the problem. Ownership follows the The Create Rule.

## Return Value

If `bundle` is already loaded, returns `true`. If `bundle` is not already loaded, attempts to load `bundle`; if that attempt succeeds returns `true`, otherwise returns `false`.

## See Also

### Loading and Unloading a Bundle

func CFBundleIsExecutableLoaded(CFBundle!) -> Bool

Obtains information about the load status for a bundle’s main executable.

func CFBundlePreflightExecutable(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded or appears to be loadable.

func CFBundleLoadExecutable(CFBundle!) -> Bool

Loads a bundle’s main executable code into memory and dynamically links it into the running application.

func CFBundleUnloadExecutable(CFBundle!)

Unloads the main executable for the specified bundle.

