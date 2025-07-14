

- Device Management
-  UserConfiguredCommand 

Device Management Command

# UserConfiguredCommand

The command to inform a Shared iPad that the system has configured the user and can allow the user to continue in Setup Assistant.

iOS 17.0+iPadOS 17.0+Device Assignment ServicesVPP License Management

``` source
object UserConfiguredCommand
```

## Properties

`Command`

UserConfiguredCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object UserConfiguredCommand.Command

## See Also

### Command and Response

object UserConfiguredResponse

A response from the Shared iPad after it processes the command to configure the user and continue in Setup Assistant.

