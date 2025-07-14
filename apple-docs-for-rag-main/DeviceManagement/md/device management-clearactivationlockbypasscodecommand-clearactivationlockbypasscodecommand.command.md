

- Device Management
- ClearActivationLockBypassCodeCommand
-  ClearActivationLockBypassCodeCommand.Command 

Device Management Command

# ClearActivationLockBypassCodeCommand.Command

The request dictionary to clear the Activation Lock bypass code on a device.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object ClearActivationLockBypassCodeCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to clear the Activation Lock bypass code on a device.

Value: `ClearActivationLockBypassCode`

