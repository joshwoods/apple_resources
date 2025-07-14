

- Device Management
-  ActivationLockBypassCodeCommand 

Device Management Command

# ActivationLockBypassCodeCommand

The command to get the code to bypass Activation Lock on a device.

iOS 7.1+iPadOS 7.1+macOS 10.15+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object ActivationLockBypassCodeCommand
```

## Properties

`Command`

ActivationLockBypassCodeCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Mentioned in 

Handling NotNow Status Responses

## Topics

### Commands

object ActivationLockBypassCodeCommand.Command

The request dictionary to get the code to bypass Activation Lock on a device.

## See Also

### Command and Response

object ActivationLockBypassCodeResponse

A response from the device after it processes the command to get the Activation Lock bypass code.

