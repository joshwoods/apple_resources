

- Device Management
-  DeviceConfiguredCommand 

Device Management Command

# DeviceConfiguredCommand

The command to inform a device that it can allow the user to continue in Setup Assistant.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 10.2+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object DeviceConfiguredCommand
```

## Properties

`Command`

DeviceConfiguredCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object DeviceConfiguredCommand.Command

The request dictionary to inform a device that it can allow the user to continue in Setup Assistant.

## See Also

### Command and Response

object DeviceConfiguredResponse

A response from the device after it processes the command to allow the user to continue in Setup Assistant.

