

- Device Management
- DeleteUserCommand
-  DeleteUserCommand.Command 

Device Management Command

# DeleteUserCommand.Command

The request dictionary to delete a user’s account from a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object DeleteUserCommand.Command
```

## Properties

`DeleteAllUsers`

`boolean`

If `true`, the system attempts to delete all users from the device. If `ForceDeletion` is `false`, the system generates an error instead and doesn’t delete users who have data that’s pending sync. This value is available in iOS 14 and later.

Default: `false`

`ForceDeletion`

`boolean`

If `true`, the system deletes the account even if the user has data that’s pending sync to the cloud. This value is available on iOS 9.3 and later.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to delete a user’s account from a device.

Value: `DeleteUser`

`UserName`

`string`

The user name of the account to delete. This key is required when the value for `DeleteAllUsers` is absent or `false`.

