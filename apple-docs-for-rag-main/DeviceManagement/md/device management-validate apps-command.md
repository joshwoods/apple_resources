

- Device Management
-  Validate Apps 

Web Service Endpoint

# Validate Apps

Force validation of developer and universal provisioning profiles for enterprise apps.

iOS 9.2+iPadOS 9.2+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ValidateApplicationsCommand
```

## HTTP Body

ValidateApplicationsCommand

The command to force validation of developer and universal provisioning profiles for enterprise apps on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ValidateApplicationsResponse

`OK`

A response from the device after it processes the command to validate provisioning profiles for enterprise apps.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Avaliability

|                            |                        |
|----------------------------|------------------------|
| Device Channel             | iOS, Shared iPad, tvOS |
| User Channel               | \-                     |
| Requires Supervision       | \-                     |
| Allowed in User Enrollment | iOS                    |
| Required Access Right      | AllowAppInstallation   |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ValidateApplications

    CommandUUID
    0001_ValidateApplications

```

```

    CommandUUID
    0001_ValidateApplications
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ValidateApplicationsCommand

The command to force validation of developer and universal provisioning profiles for enterprise apps on a device.

object ValidateApplicationsResponse

A response from the device after it processes the command to validate provisioning profiles for enterprise apps.

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

List the Managed Apps

Get the status of all managed apps on a device.

Query App Attributes

Query attributes in managed apps on a device.

Get App Configuration

Get app configurations from managed apps on a device.

Get App Feedback

Get app feedback from a managed app on the device.

