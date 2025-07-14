

- Device Management
-  ManagedApplicationConfigurationCommand 

Device Management Command

# ManagedApplicationConfigurationCommand

The command to get managed app configurations on a device.

iOS 7.0+iPadOS 7.0+macOS 10.15+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationConfigurationCommand
```

## Properties

`Command`

ManagedApplicationConfigurationCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ManagedApplicationConfigurationCommand.Command

The request dictionary to get managed app configurations.

## See Also

### Command and Response

object ManagedApplicationConfigurationResponse

A response from the device after it processes the command to get app configurations from managed apps.

