

- Device Management
-  List the Installed Profiles 

Web Service Endpoint

# List the Installed Profiles

Get a list of installed profiles on a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ProfileListCommand
```

## HTTP Body

ProfileListCommand

The command to get a list of installed profiles on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ProfileListResponse

`OK`

A response from the device after it processes the command to get a list of installed profiles.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS, Shared iPad                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowInspection                        |

### Example Request and Response

- Request
- Response

```

    Command

        ManagedOnly

        RequestType
        ProfileList

    CommandUUID
    0001_ProfileList

```

```

    CommandUUID
    0001_ProfileList
    ProfileList

            HasRemovalPasscode

            IsEncrypted

            IsManaged

            PayloadContent

                    PayloadDescription
                    Installs a PEM certificate payload.
                    PayloadDisplayName
                    PEM certificate payload
                    PayloadIdentifier
                    com.apple.security.pem.ea74b673-50b9-498c-8314-5cfef174d102
                    PayloadOrganization
                    Acme, Inc.
                    PayloadType
                    com.apple.security.pem
                    PayloadVersion
                    1

                    PayloadDescription
                    Enrolls your device into SCEP on this MDM server.
                    PayloadDisplayName
                    MDM SCEP payload
                    PayloadIdentifier
                    com.apple.security.scep.aa48bb57-e657-4a87-b6b0-6f5159055304
                    PayloadOrganization
                    Acme, Inc.
                    PayloadType
                    com.apple.security.scep
                    PayloadVersion
                    1

                    PayloadDescription
                    Enrolls your device into this MDM server.
                    PayloadDisplayName
                    MDM
                    PayloadIdentifier
                    com.apple.mdm.4e86d728-2c38-4410-bea2-fbe4b77619e3
                    PayloadOrganization
                    Acme, Inc.
                    PayloadType
                    com.apple.mdm
                    PayloadVersion
                    1

            PayloadDescription
            Enrolls your device into this MDM server.
            PayloadDisplayName
            Python MDM
            PayloadIdentifier
            com.acme.mdm.mdm
            PayloadOrganization
            Acme, Inc.
            PayloadRemovalDisallowed

            PayloadUUID
            a96f429c-d881-47e7-ad07-eeca163976fb
            PayloadVersion
            1

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ProfileListCommand

The command to get a list of installed profiles on a device.

object ProfileListResponse

A response from the device after it processes the command to get a list of installed profiles.

## See Also

### Profile Management

Install a Profile

Install a configuration profile on a device.

Remove a Profile

Remove a previously installed profile from the device.

Install a Provisioning Profile

Install a provisioning profile on a device.

List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.

