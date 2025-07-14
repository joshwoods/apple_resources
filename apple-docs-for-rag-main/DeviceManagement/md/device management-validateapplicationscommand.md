

- Device Management
-  ValidateApplicationsCommand 

Device Management Command

# ValidateApplicationsCommand

The command to force validation of developer and universal provisioning profiles for enterprise apps on a device.

iOS 9.2+iPadOS 9.2+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ValidateApplicationsCommand
```

## Properties

`Command`

ValidateApplicationsCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ValidateApplicationsCommand.Command

The request dictionary to validate provisioning profiles for enterprise apps.

## See Also

### Command and Response

object ValidateApplicationsResponse

A response from the device after it processes the command to validate provisioning profiles for enterprise apps.

