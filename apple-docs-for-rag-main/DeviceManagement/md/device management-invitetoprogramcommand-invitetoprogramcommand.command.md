

- Device Management
- InviteToProgramCommand
-  InviteToProgramCommand.Command 

Device Management Command

# InviteToProgramCommand.Command

The request dictionary to invite a user to join the Volume Purchase Program (VPP).

iOS 7.0+iPadOS 7.0+macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object InviteToProgramCommand.Command
```

## Properties

`InvitationURL`

`string`

 (Required) 

The Volume Purchase Program (VPP) invitation URL.

`ProgramID`

`string`

 (Required) 

The program’s identifier, which can only be `com.apple.cloudvpp`.

Value: `com.apple.cloudvpp`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to invite a user to join the Volume Purchase Program (VPP).

Value: `InviteToProgram`

