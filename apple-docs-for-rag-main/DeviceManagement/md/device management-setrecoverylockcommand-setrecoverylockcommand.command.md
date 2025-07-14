

- Device Management
- SetRecoveryLockCommand
-  SetRecoveryLockCommand.Command 

Device Management Command

# SetRecoveryLockCommand.Command

The request dictionary to set the Recovery Lock password.

macOS 11.5+Device Assignment ServicesVPP License Management

``` source
object SetRecoveryLockCommand.Command
```

## Properties

`CurrentPassword`

`string`

If the device has a Recovery Lock password set, the system requires the current password.

`NewPassword`

`string`

 (Required) 

The new password for Recovery Lock. Set as an empty string to clear the Recovery Lock password.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to set the Recovery Lock password.

Value: `SetRecoveryLock`

