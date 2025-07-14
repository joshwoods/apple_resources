

- Core Media I/O
- CMIOExtensionDevice
-  init(localizedName:deviceID:source:) 

Initializer

# init(localizedName:deviceID:source:)

Creates an extension device.

Mac Catalyst 15.4+

``` source
convenience init(
    localizedName: String,
    deviceID: UUID,
    source: any CMIOExtensionDeviceSource
)
```

## Parameters 

`localizedName`  

A localized name for the device.

`deviceID`  

A universally unique device identifier value.

`source`  

An extension-specific object that conforms to the CMIOExtensionDeviceSource protocol.

## See Also

### Creating a Device

init(localizedName: String, deviceID: UUID, legacyDeviceID: String?, source: any CMIOExtensionDeviceSource)

Creates an extension device with an optional legacy device identifier.

