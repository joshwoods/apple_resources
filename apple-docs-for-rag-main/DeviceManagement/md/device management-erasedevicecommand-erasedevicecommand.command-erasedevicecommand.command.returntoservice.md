

- Device Management
- EraseDeviceCommand
- EraseDeviceCommand.Command
-  EraseDeviceCommand.Command.ReturnToService 

Device Management Command

# EraseDeviceCommand.Command.ReturnToService

The configuration settings for Return to Service.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object EraseDeviceCommand.Command.ReturnToService
```

## Properties

`Enabled`

`boolean`

 (Required) 

If `true`, the device tries to re-enroll itself automatically after erasure. The user needs to deactivate all activation locks for this feature to work correctly.

`MDMProfileData`

`data`

The MDM profile installed after erasure, when using Return to Service. This key is required for all unsupervised devices, as well as supervised devices that weren’t enrolled with ADE. If provided, the device uses this profile directly instead of fetching it from the server. For ADE enrolled devices, this key isn’t necessary unless the cloud configuration profile of the device contains the `configuration-web-url` key.

The cloud configuration is still downloaded from Apple’s servers when the profile contains this key, so the supervision identity, MDM removability and other settings from the cloud configuration still applies. However, the device doesn’t use the URL specified in the cloud configuration to fetch the MDM profile.

`WiFiProfileData`

`data`

The WiFi profile that installed after erasure, when using Return to Service. This is required when the device doesn’t have ethernet access.

## Discussion

This command is available in iOS 17 and later and with Shared iPad.

