

- Core Foundation
-  CFBundlePreflightExecutable(\_:\_:) 

Function

# CFBundlePreflightExecutable(\_:\_:)

Returns a Boolean value that indicates whether a given bundle is loaded or appears to be loadable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFBundlePreflightExecutable(
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

`true` if `bundle` is loaded or upon inspection appears to be loadable, otherwise `false`.

## Discussion

If this function returns true, this does not mean that the bundle is definitively loadable, since it may fail to load due to link errors or other problems not readily detectable.

## See Also

### Loading and Unloading a Bundle

func CFBundleIsExecutableLoaded(CFBundle!) -> Bool

Obtains information about the load status for a bundle’s main executable.

func CFBundleLoadExecutable(CFBundle!) -> Bool

Loads a bundle’s main executable code into memory and dynamically links it into the running application.

func CFBundleLoadExecutableAndReturnError(CFBundle!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns a Boolean value that indicates whether a given bundle is loaded, attempting to load it if necessary.

func CFBundleUnloadExecutable(CFBundle!)

Unloads the main executable for the specified bundle.

