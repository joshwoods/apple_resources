

- Device Management
-  ManagedApplicationAttributesCommand 

Device Management Command

# ManagedApplicationAttributesCommand

The command to query managed app attributes on a device.

iOS 7.0+iPadOS 7.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationAttributesCommand
```

## Properties

`Command`

ManagedApplicationAttributesCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ManagedApplicationAttributesCommand.Command

The request dictionary to query managed app attributes.

## See Also

### Command and Response

object ManagedApplicationAttributesResponse

A response from the device after it processes the command to query attributes in managed apps.

