

- Core Foundation
-  CFPlugInIsLoadOnDemand(\_:) 

Function

# CFPlugInIsLoadOnDemand(\_:)

Determines whether or not a plug-in is loaded on demand.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInIsLoadOnDemand(_ plugIn: CFPlugIn!) -> Bool
```

## Parameters 

`plugIn`  

The plug-in to query.

## Return Value

`true` if the plug-in is loaded only when a client requests an instance of a supported type, otherwise `false`.

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

func CFPlugInRemoveInstanceForFactory(CFUUID!)

Unregisters an instance of a type with `CFPlugIn`.

func CFPlugInSetLoadOnDemand(CFPlugIn!, Bool)

Enables or disables load on demand for plug-ins that do dynamic registration (only when a client requests an instance of a supported type).

