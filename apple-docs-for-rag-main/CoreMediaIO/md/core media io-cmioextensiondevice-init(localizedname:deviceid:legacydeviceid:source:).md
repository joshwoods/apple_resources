

- Core Media I/O
- CMIOExtensionDevice
-  init(localizedName:deviceID:legacyDeviceID:source:) 

Initializer

# init(localizedName:deviceID:legacyDeviceID:source:)

Creates an extension device with an optional legacy device identifier.

Mac Catalyst 15.4+macOS 12.3+

``` source
init(
    localizedName: String,
    deviceID: UUID,
    legacyDeviceID: String?,
    source: any CMIOExtensionDeviceSource
)
```

## Parameters 

`localizedName`  

A localized name for the device.

`deviceID`  

A universally unique device identifier value.

`legacyDeviceID`  

A string device identifier for backward compatibility with existing CMIO DAL clients. The value you provide can differ from the value of `deviceID.UUIDString`.

Set this argument to `nil` if your device has no backward-compatibility requirements.

`source`  

An extension-specific object that conforms to the CMIOExtensionDeviceSource protocol.

## See Also

### Creating a Device

convenience init(localizedName: String, deviceID: UUID, source: any CMIOExtensionDeviceSource)

Creates an extension device.

