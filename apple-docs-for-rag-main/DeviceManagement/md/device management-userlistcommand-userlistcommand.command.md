

- Device Management
- UserListCommand
-  UserListCommand.Command 

Device Management Command

# UserListCommand.Command

The request dictionary to get a list of users with active accounts on a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object UserListCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of users with active accounts on a device.

Value: `UserList`

