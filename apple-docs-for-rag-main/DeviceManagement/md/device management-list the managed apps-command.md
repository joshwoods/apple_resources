

- Device Management
-  List the Managed Apps 

Web Service Endpoint

# List the Managed Apps

Get the status of all managed apps on a device.

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ManagedApplicationListCommand
```

## HTTP Body

ManagedApplicationListCommand

The command to get the status of managed apps on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ManagedApplicationListResponse

`OK`

A response from the device after it processes the command to get the status of all managed apps.

Content-Type: application/xml

## Discussion

This command returns the status of managed apps from the App Store.

Some statuses are transient and the device removes them after reporting them to the server.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowAppInstallation                   |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ManagedApplicationList

    CommandUUID
    0001_ManagedApplicationList

```

```

    CommandUUID
    0080_ManagedApplicationList
    ManagedApplicationList

        com.acme.myenterpriseapp

            ExternalVersionIdentifier
            0
            HasConfiguration

            HasFeedback

            IsValidated

            ManagementFlags
            0
            Status
            Managed

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ManagedApplicationListCommand

The command to get the status of managed apps on a device.

object ManagedApplicationListResponse

A response from the device after it processes the command to get the status of all managed apps.

## See Also

### Managed Apps

Install an App

Install a third-party app on a device.

Install an Enterprise App

Install an enterprise app on a device.

Apply a Redemption Code

Complete the installation of an app using a redemption code.

Remove an App

Remove an installed managed app.

Validate Apps

Force validation of developer and universal provisioning profiles for enterprise apps.

Query App Attributes

Query attributes in managed apps on a device.

Get App Configuration

Get app configurations from managed apps on a device.

Get App Feedback

Get app feedback from a managed app on the device.

