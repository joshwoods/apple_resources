

- Core Foundation
-  CFPlugInRegisterFactoryFunctionByName(\_:\_:\_:) 

Function

# CFPlugInRegisterFactoryFunctionByName(\_:\_:\_:)

Registers a factory function with a `CFPlugIn` object using the function’s name instead of its UUID.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInRegisterFactoryFunctionByName(
    _ factoryUUID: CFUUID!,
    _ plugIn: CFPlugIn!,
    _ functionName: CFString!
) -> Bool
```

## Parameters 

`factoryUUID`  

The `CFUUID` object representing the factory function to register.

`plugIn`  

The plug-in containing `functionName`.

`functionName`  

The name of the factory function to register.

## Return Value

`true` if the factory function was successfully registered, otherwise `false`.

## Discussion

This function is used by a plug-in or host when performing dynamic registration.

## See Also

### Registration

func CFPlugInRegisterFactoryFunction(CFUUID!, CFPlugInFactoryFunction!) -> Bool

Registers a factory function and its UUID with a `CFPlugIn` object.

func CFPlugInRegisterPlugInType(CFUUID!, CFUUID!) -> Bool

Registers a type and its corresponding factory function with a `CFPlugIn` object.

func CFPlugInUnregisterFactory(CFUUID!) -> Bool

Removes the given function from a plug-in’s list of registered factory functions.

func CFPlugInUnregisterPlugInType(CFUUID!, CFUUID!) -> Bool

Removes the given type from a plug-in’s list of registered types.

