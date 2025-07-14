

- Device Management
-  ManagedApplicationFeedbackCommand 

Device Management Command

# ManagedApplicationFeedbackCommand

The command to get managed app feedback on a device.

iOS 7.0+iPadOS 7.0+macOS 11.0+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationFeedbackCommand
```

## Properties

`Command`

ManagedApplicationFeedbackCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ManagedApplicationFeedbackCommand.Command

The request dictionary to get managed app feedback.

## See Also

### Command and Response

object ManagedApplicationFeedbackResponse

A response from the device after it processes the command to get app feedback from a managed app.

