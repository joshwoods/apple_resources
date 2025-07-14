

- Core Foundation
-  CFPlugInFindFactoriesForPlugInType(\_:) 

Function

# CFPlugInFindFactoriesForPlugInType(\_:)

Searches all registered plug-ins for factory functions capable of creating an instance of the given type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInFindFactoriesForPlugInType(_ typeUUID: CFUUID!) -> CFArray!
```

## Parameters 

`typeUUID`  

A UUID type.

## Return Value

An array of UUIDs for factory functions capable of creating an instance of the given type.

## See Also

### CFPlugIn Miscellaneous Functions

func CFPlugInAddInstanceForFactory(CFUUID!)

Registers a new instance of a type with `CFPlugIn`.

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

func CFPlugInSetLoadOnDemand(CFPlugIn!, Bool)

Enables or disables load on demand for plug-ins that do dynamic registration (only when a client requests an instance of a supported type).

