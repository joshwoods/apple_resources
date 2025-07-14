

- Device Management
-  ClearPasscodeCommand 

Device Management Command

# ClearPasscodeCommand

The command to clear the passcode on a device.

iOS 4.0+iPadOS 4.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ClearPasscodeCommand
```

## Properties

`Command`

ClearPasscodeCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Mentioned in 

Managing Passcodes

Handling NotNow Status Responses

## Topics

### Commands

object ClearPasscodeCommand.Command

The request dictionary to clear a passcode.

## See Also

### Command and Response

object ClearPasscodeResponse

A response from the device after it processes the command to remove the passcode from a device.

