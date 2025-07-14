

- Core Foundation
-  CFPlugInUnregisterPlugInType(\_:\_:) 

Function

# CFPlugInUnregisterPlugInType(\_:\_:)

Removes the given type from a plug-in’s list of registered types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInUnregisterPlugInType(
    _ factoryUUID: CFUUID!,
    _ typeUUID: CFUUID!
) -> Bool
```

## Parameters 

`factoryUUID`  

The `CFUUID` object representing the factory function for the type to unregister.

`typeUUID`  

The UUID type to unregister.

## Return Value

`true` if the factory function was successfully unregistered, otherwise `false`.

## Discussion

Used by a plug-in or host when performing dynamic registration.

## See Also

### Registration

func CFPlugInRegisterFactoryFunction(CFUUID!, CFPlugInFactoryFunction!) -> Bool

Registers a factory function and its UUID with a `CFPlugIn` object.

func CFPlugInRegisterFactoryFunctionByName(CFUUID!, CFPlugIn!, CFString!) -> Bool

Registers a factory function with a `CFPlugIn` object using the function’s name instead of its UUID.

func CFPlugInRegisterPlugInType(CFUUID!, CFUUID!) -> Bool

Registers a type and its corresponding factory function with a `CFPlugIn` object.

func CFPlugInUnregisterFactory(CFUUID!) -> Bool

Removes the given function from a plug-in’s list of registered factory functions.

