

- Device Management
-  List the Installed Provisioning Profiles 

Web Service Endpoint

# List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ProvisioningProfileListCommand
```

## HTTP Body

ProvisioningProfileListCommand

The command to get a list of installed provisioning profiles on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ProvisioningProfileListResponse

`OK`

A response from the device after it processes the command to get a list of its provisioning profiles.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS                                    |
| Required Access Right      | AllowProvisioningInspection            |

### Example Request and Response

- Request
- Response

```

    Command

        ManagedOnly

        RequestType
        ProvisioningProfileList

    CommandUUID
    0001_ProvisioningProfileList

```

```

    CommandUUID
    0001_ProvisioningProfileList
    ProvisioningProfileList

            ExpiryDate
            2020-02-12T20:58:40Z
            Name
            My Company (February 2019 - February 2020)
            UUID
            493d9dc8-e4c0-4fd8-bd8e-8fd4c0dc7b0c

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ProvisioningProfileListCommand

The command to get a list of installed provisioning profiles on a device.

object ProvisioningProfileListResponse

A response from the device after it processes the command to get a list of its provisioning profiles.

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

Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.

