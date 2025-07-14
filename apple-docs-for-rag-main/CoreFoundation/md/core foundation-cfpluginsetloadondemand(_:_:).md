

- Core Foundation
-  CFPlugInSetLoadOnDemand(\_:\_:) 

Function

# CFPlugInSetLoadOnDemand(\_:\_:)

Enables or disables load on demand for plug-ins that do dynamic registration (only when a client requests an instance of a supported type).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInSetLoadOnDemand(
    _ plugIn: CFPlugIn!,
    _ flag: Bool
)
```

## Parameters 

`plugIn`  

The plug-in to be loaded on demand.

`flag`  

`true` to enable load on demand, `false` otherwise.

## Discussion

Plug-ins that do static registration are load on demand by default. Plug-ins that do dynamic registration are not load on demand by default.

## See Also

### CFPlugIn Miscellaneous Functions

func CFPlugInAddInstanceForFactory(CFUUID!)

Registers a new instance of a type with `CFPlugIn`.

func CFPlugInFindFactoriesForPlugInType(CFUUID!) -> CFArray!

Searches all registered plug-ins for factory functions capable of creating an instance of the given type.

func CFPlugInFindFactoriesForPlugInTypeInPlugIn(CFUUID!, CFPlugIn!) -> CFArray!

Searches the given plug-in for factory functions capable of creating an instance of the given type.

func CFPlugInGetBundle(CFPlugIn!) -> CFBundle!

Returns a plug-in’s bundle.

func CFPlugInGetTypeID() -> CFTypeID

Returns the type identifier for the `CFPlugIn` opaque type.

func CFPlugInIsLoadOnDemand(CFPlugIn!) -> Bool

Determines whether or not a plug-in is loaded on demand.

func CFPlugInRemoveInstanceForFactory(CFUUID!)

Unregisters an instance of a type with `CFPlugIn`.

