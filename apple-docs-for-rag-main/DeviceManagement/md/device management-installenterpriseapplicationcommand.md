

- Device Management
-  InstallEnterpriseApplicationCommand 

Device Management Command

# InstallEnterpriseApplicationCommand

The command to install an enterprise app on a device.

macOS 10.13.6+Device Assignment ServicesVPP License Management

``` source
object InstallEnterpriseApplicationCommand
```

## Properties

`Command`

InstallEnterpriseApplicationCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Discussion

This command provides a more secure version of InstallApplicationCommand that specifies a InstallEnterpriseApplicationCommand.Command.Manifest or ManifestURL.

The request needs to contain either a `Manifest` or `ManifestURL`. When using `Manifest`, the system ignores pinning options. When using `ManifestURL`, it’s recommended to specify the pinning options to increase security.

In macOS, the system returns `Acknowledged` after it validates the parameters but before it downloads and installs the app. As a result, the system won’t report errors in the installation process to the MDM server.

## Topics

### Commands

object InstallEnterpriseApplicationCommand.Command

The request dictionary to install an enterprise app.

## See Also

### Command and Response

object InstallEnterpriseApplicationResponse

A response from the device after it processes the command to install an enterprise app.

