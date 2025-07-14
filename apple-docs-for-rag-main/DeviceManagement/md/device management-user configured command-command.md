

- Device Management
-  User Configured Command 

Web Service Endpoint

# User Configured Command

Informs the device that it can continue past Setup Assistant and finish login.

iOS 17.0+iPadOS 17.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#UserConfiguredCommand
```

## HTTP Body

UserConfiguredCommand

missing

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

UserConfiguredResponse

`OK`

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements.

### Command Availability

|                            |             |
|----------------------------|-------------|
| Device Channel             | \-          |
| User Channel               | Shared iPad |
| Requires Supervision       | Shared iPad |
| Allowed in User Enrollment | \-          |
| Required Access Right      | \-          |

## Topics

### Command and Response

object UserConfiguredCommand

The command to inform a Shared iPad that the system has configured the user and can allow the user to continue in Setup Assistant.

object UserConfiguredResponse

A response from the Shared iPad after it processes the command to configure the user and continue in Setup Assistant.

## See Also

### Device Details

List the Installed Apps

Get a list of the installed apps on a device.

Get Device Information

Get detailed information about a device.

Release Device from Await Configuration

Inform the device that it can allow the user to continue in Setup Assistant.

List the Installed Restrictions

Get a list of restrictions on the device.

