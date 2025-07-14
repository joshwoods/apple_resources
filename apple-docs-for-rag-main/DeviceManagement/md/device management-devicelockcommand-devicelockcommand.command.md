

- Device Management
- DeviceLockCommand
-  DeviceLockCommand.Command 

Device Management Command

# DeviceLockCommand.Command

The request dictionary to lock a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceLockCommand.Command
```

## Properties

`Message`

`string`

The message to display on the Lock screen of the device. This value doesn’t apply to a shared iPad device. This value is available in iOS 4 and later, and macOS 10.14 and later.

`PhoneNumber`

`string`

The phone number to display on the Lock screen. This value doesn’t apply to a shared iPad device. This value is available in iOS 7 and later and macOS 11.5 and later (for Apple silicon devices only).

`PIN`

`string`

The six-character PIN for Find My. This value is available in macOS 10.8 and later.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to lock a device.

Value: `DeviceLock`

