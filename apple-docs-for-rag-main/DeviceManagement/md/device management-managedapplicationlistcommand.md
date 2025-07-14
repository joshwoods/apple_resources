

- Device Management
-  ManagedApplicationListCommand 

Device Management Command

# ManagedApplicationListCommand

The command to get the status of managed apps on a device.

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationListCommand
```

## Properties

`Command`

ManagedApplicationListCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ManagedApplicationListCommand.Command

The request dictionary to get the status of managed apps.

## See Also

### Command and Response

object ManagedApplicationListResponse

A response from the device after it processes the command to get the status of all managed apps.

