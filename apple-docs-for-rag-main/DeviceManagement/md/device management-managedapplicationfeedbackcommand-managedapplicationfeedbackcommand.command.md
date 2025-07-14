

- Device Management
- ManagedApplicationFeedbackCommand
-  ManagedApplicationFeedbackCommand.Command 

Device Management Command

# ManagedApplicationFeedbackCommand.Command

The request dictionary to get managed app feedback.

iOS 7.0+iPadOS 7.0+macOS 11.0+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationFeedbackCommand.Command
```

## Properties

`Identifiers`

`[string]`

 (Required) 

The bundle identifiers of the managed apps.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get managed app feedback.

Value: `ManagedApplicationFeedback`

`DeleteFeedback`

`boolean`

If `true`, delete the app’s feedback dictionary after the server reads it.

Default: `false`

