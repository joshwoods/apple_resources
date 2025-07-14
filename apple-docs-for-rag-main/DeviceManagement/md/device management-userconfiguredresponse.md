

- Device Management
-  UserConfiguredResponse 

Device Management Command

# UserConfiguredResponse

A response from the Shared iPad after it processes the command to configure the user and continue in Setup Assistant.

iOS 17.0+iPadOS 17.0+Device Assignment ServicesVPP License Management

``` source
object UserConfiguredResponse
```

## Properties

`CommandUUID`

`string`

`EnrollmentID`

`string`

 (Required) 

`EnrollmentUserID`

`string`

 (Required) 

`ErrorChain`

`[`UserConfiguredResponse.ErrorChainItem`]`

`NotOnConsole`

`boolean`

 (Required) 

`Status`

`string`

 (Required) 

Possible Values: `Acknowledged, Error, CommandFormatError, Idle, NotNow`

`UDID`

`string`

 (Required) 

`UserID`

`string`

`UserLongName`

`string`

 (Required) 

`UserShortName`

`string`

## Topics

### Commands

object UserConfiguredResponse.ErrorChainItem

## See Also

### Command and Response

object UserConfiguredCommand

The command to inform a Shared iPad that the system has configured the user and can allow the user to continue in Setup Assistant.

