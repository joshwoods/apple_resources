

- Device Management
- InstalledApplicationListCommand
-  InstalledApplicationListCommand.Command 

Device Management Command

# InstalledApplicationListCommand.Command

The request dictionary to get a list of installed apps.

iOS 5.0+iPadOS 5.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstalledApplicationListCommand.Command
```

## Properties

`Identifiers`

`[string]`

An array of app identifiers. Provide this value to limit the response to only include these apps. This value is available in iOS 7 and later, macOS 10.15 and later, and tvOS 10.2 and later.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of installed apps.

Value: `InstalledApplicationList`

`ManagedAppsOnly`

`boolean`

If `true`, only get a list of managed apps. This value is available in iOS 7 and later, macOS 10.15 and later, and tvOS 10.2 and later.

Default: `false`

`Items`

`[string]`

An array of strings that represent keys in InstalledApplicationListResponse.InstalledApplicationListItem. If present, the response only contains the keys listed here, except `Identifier` is always included. If not present, the response contains all keys.

Tip

Only request the keys that you need, because some key values can take significant time and power to calculate on the device.

Possible Values: `AdHocCodeSigned, AppStoreVendable, BetaApp, BundleSize, DeviceBasedVPP, DistributorIdentifier, DynamicSize, ExternalVersionIdentifier, HasUpdateAvailable, Identifier, Installing, IsAppClip, IsValidated, Name, ShortVersion, Version`

