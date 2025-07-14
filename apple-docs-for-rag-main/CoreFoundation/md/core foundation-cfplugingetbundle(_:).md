

- Core Foundation
-  CFPlugInGetBundle(\_:) 

Function

# CFPlugInGetBundle(\_:)

Returns a plug-in’s bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInGetBundle(_ plugIn: CFPlugIn!) -> CFBundle!
```

## Parameters 

`plugIn`  

The plug-in whose bundle to obtain.

## Return Value

The bundle for `plugIn`. Ownership follows the The Get Rule.

## Discussion

You should *always* use this function to get a plug-in’s bundle. Never attempt to access the plug-in directly as a bundle.

## See Also

### CFPlugIn Miscellaneous Functions

func CFPlugInAddInstanceForFactory(CFUUID!)

Registers a new instance of a type with `CFPlugIn`.

func CFPlugInFindFactoriesForPlugInType(CFUUID!) -> CFArray!

Searches all registered plug-ins for factory functions capable of creating an instance of the given type.

func CFPlugInFindFactoriesForPlugInTypeInPlugIn(CFUUID!, CFPlugIn!) -> CFArray!

Searches the given plug-in for factory functions capable of creating an instance of the given type.

func CFPlugInGetTypeID() -> CFTypeID

Returns the type identifier for the `CFPlugIn` opaque type.

func CFPlugInIsLoadOnDemand(CFPlugIn!) -> Bool

Determines whether or not a plug-in is loaded on demand.

func CFPlugInRemoveInstanceForFactory(CFUUID!)

Unregisters an instance of a type with `CFPlugIn`.

func CFPlugInSetLoadOnDemand(CFPlugIn!, Bool)

Enables or disables load on demand for plug-ins that do dynamic registration (only when a client requests an instance of a supported type).

