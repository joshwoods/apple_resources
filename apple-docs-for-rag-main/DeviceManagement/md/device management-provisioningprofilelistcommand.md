

- Device Management
-  ProvisioningProfileListCommand 

Device Management Command

# ProvisioningProfileListCommand

The command to get a list of installed provisioning profiles on a device.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProvisioningProfileListCommand
```

## Properties

`Command`

ProvisioningProfileListCommand.Command

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

object ProvisioningProfileListCommand.Command

The request dictionary to get a list of installed provisioning profiles.

## See Also

### Command and Response

object ProvisioningProfileListResponse

A response from the device after it processes the command to get a list of its provisioning profiles.

