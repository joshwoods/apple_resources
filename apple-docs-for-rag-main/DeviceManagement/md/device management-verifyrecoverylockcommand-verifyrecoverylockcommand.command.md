

- Device Management
- VerifyRecoveryLockCommand
-  VerifyRecoveryLockCommand.Command 

Device Management Command

# VerifyRecoveryLockCommand.Command

The request dictionary to verify the Recovery Lock password.

macOS 11.5+Device Assignment ServicesVPP License Management

``` source
object VerifyRecoveryLockCommand.Command
```

## Properties

`Password`

`string`

 (Required) 

The password to verify.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to verify the Recovery Lock password.

Value: `VerifyRecoveryLock`

