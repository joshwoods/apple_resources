

- Device Management
-  Remove a Provisioning Profile 

Web Service Endpoint

# Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RemoveProvisioningProfileCommand
```

## HTTP Body

RemoveProvisioningProfileCommand

The command to remove a provisioning profile from a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RemoveProvisioningProfileResponse

`OK`

A response from the device after it processes the command to remove a provisioning profile.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS                                    |
| Required Access Right      | AllowProvisioningInstallationRemoval   |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        RemoveProvisioningProfile
        UUID
        493d9dc8-e4c0-4fd8-bd8e-8fd4c0dc7b0c

    CommandUUID
    0001_RemoveProvisioningProfile

```

```

    CommandUUID
    0001_RemoveProvisioningProfile
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RemoveProvisioningProfileCommand

The command to remove a provisioning profile from a device.

object RemoveProvisioningProfileResponse

A response from the device after it processes the command to remove a provisioning profile.

## See Also

### Profile Management

Install a Profile

Install a configuration profile on a device.

List the Installed Profiles

Get a list of installed profiles on a device.

Remove a Profile

Remove a previously installed profile from the device.

Install a Provisioning Profile

Install a provisioning profile on a device.

List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

