

- Core Foundation
-  CFPlugInRegisterPlugInType(\_:\_:) 

Function

# CFPlugInRegisterPlugInType(\_:\_:)

Registers a type and its corresponding factory function with a `CFPlugIn` object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInRegisterPlugInType(
    _ factoryUUID: CFUUID!,
    _ typeUUID: CFUUID!
) -> Bool
```

## Parameters 

`factoryUUID`  

The `CFUUID` object representing the factory function that can create the type being registered.

`typeUUID`  

The UUID type to register.

## Return Value

`true` if the factory function was successfully registered, otherwise `false`.

## Discussion

This function is used by a plug-in or host when performing dynamic registration.

## See Also

### Registration

func CFPlugInRegisterFactoryFunction(CFUUID!, CFPlugInFactoryFunction!) -> Bool

Registers a factory function and its UUID with a `CFPlugIn` object.

func CFPlugInRegisterFactoryFunctionByName(CFUUID!, CFPlugIn!, CFString!) -> Bool

Registers a factory function with a `CFPlugIn` object using the function’s name instead of its UUID.

func CFPlugInUnregisterFactory(CFUUID!) -> Bool

Removes the given function from a plug-in’s list of registered factory functions.

func CFPlugInUnregisterPlugInType(CFUUID!, CFUUID!) -> Bool

Removes the given type from a plug-in’s list of registered types.

