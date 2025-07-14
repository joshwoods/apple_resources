

- Device Management
- ActivationLockBypassCodeCommand
-  ActivationLockBypassCodeCommand.Command 

Device Management Command

# ActivationLockBypassCodeCommand.Command

The request dictionary to get the code to bypass Activation Lock on a device.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object ActivationLockBypassCodeCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get the code to bypass Activation Lock on a device.

Value: `ActivationLockBypassCode`

