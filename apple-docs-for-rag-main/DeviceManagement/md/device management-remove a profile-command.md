

- Device Management
-  Remove a Profile 

Web Service Endpoint

# Remove a Profile

Remove a previously installed profile from the device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RemoveProfileCommand
```

## HTTP Body

RemoveProfileCommand

The command to remove a profile from a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RemoveProfileResponse

`OK`

A response from the device after it processes the command to remove a profile.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

Note

Don’t remove a provisioning profile to revoke access to an enterprise app. An app continues to be usable until the device restarts, even with no provisioning profile. Provisioning profiles also synchronize with iTunes and the system reinstalls them when users sync devices. For more information on removing apps, see Remove an App.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS, Shared iPad                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowInstallationRemoval               |

### Example Request and Response

- Request
- Response

```

    Command

        Identifier
        com.acme.myprofile
        RequestType
        RemoveProfile

    CommandUUID
    0001_RemoveProfile

```

```

    CommandUUID
    0001_RemoveProfile
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RemoveProfileCommand

The command to remove a profile from a device.

object RemoveProfileResponse

A response from the device after it processes the command to remove a profile.

## See Also

### Profile Management

Install a Profile

Install a configuration profile on a device.

List the Installed Profiles

Get a list of installed profiles on a device.

Install a Provisioning Profile

Install a provisioning profile on a device.

List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.

