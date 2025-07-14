

- Device Management
- UnlockUserAccountCommand
-  UnlockUserAccountCommand.Command 

Device Management Command

# UnlockUserAccountCommand.Command

The request dictionary to unlock a local user account.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object UnlockUserAccountCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to unlock a local user account.

Value: `UnlockUserAccount`

`UserName`

`string`

 (Required) 

The user name of the local account, which can be any local account on the system, not just a managed user account.

