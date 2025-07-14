

- Device Management
- LogOutUserCommand
-  LogOutUserCommand.Command 

Device Management Command

# LogOutUserCommand.Command

The request dictionary to force the current user to log out of a device.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object LogOutUserCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to force the current user to log out of a device.

Value: `LogOutUser`

