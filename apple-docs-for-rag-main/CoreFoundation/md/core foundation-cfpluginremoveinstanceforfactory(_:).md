

- Core Foundation
-  CFPlugInRemoveInstanceForFactory(\_:) 

Function

# CFPlugInRemoveInstanceForFactory(\_:)

Unregisters an instance of a type with `CFPlugIn`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInRemoveInstanceForFactory(_ factoryID: CFUUID!)
```

## Parameters 

`factoryID`  

The `CFUUID` object representing the plug-in factory.

## Discussion

If the instance counts of every factory in a plug-in are zero, the plug-in can be unloaded.

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

func CFPlugInSetLoadOnDemand(CFPlugIn!, Bool)

Enables or disables load on demand for plug-ins that do dynamic registration (only when a client requests an instance of a supported type).

