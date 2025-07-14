

- Device Management
-  Remove an App 

Web Service Endpoint

# Remove an App

Remove an installed managed app.

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RemoveApplicationCommand
```

## HTTP Body

RemoveApplicationCommand

The command to remove an installed managed app from a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RemoveApplicationResponse

`OK`

A response from the device after it processes the command to remove a managed app.

Content-Type: application/xml

## Discussion

This command only applies to managed apps and also removes the data for the removed app.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS                                    |
| Required Access Right      | AllowAppInstallation                   |

### Example Request and Response

- Request
- Response

```

    Command

        Identifier
        com.acme.myenterpriseapp
        RequestType
        RemoveApplication

    CommandUUID
    0001_RemoveApplication

```

```

    CommandUUID
    0001_RemoveApplication
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RemoveApplicationCommand

The command to remove an installed managed app from a device.

object RemoveApplicationResponse

A response from the device after it processes the command to remove a managed app.

## See Also

### Managed Apps

Install an App

Install a third-party app on a device.

Install an Enterprise App

Install an enterprise app on a device.

Apply a Redemption Code

Complete the installation of an app using a redemption code.

Validate Apps

Force validation of developer and universal provisioning profiles for enterprise apps.

List the Managed Apps

Get the status of all managed apps on a device.

Query App Attributes

Query attributes in managed apps on a device.

Get App Configuration

Get app configurations from managed apps on a device.

Get App Feedback

Get app feedback from a managed app on the device.

