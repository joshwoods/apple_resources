

- Device Management
-  Get App Feedback 

Web Service Endpoint

# Get App Feedback

Get app feedback from a managed app on the device.

iOS 7.0+iPadOS 7.0+macOS 11.0+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ManagedApplicationFeedbackCommand
```

## HTTP Body

ManagedApplicationFeedbackCommand

The command to get managed app feedback on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ManagedApplicationFeedbackResponse

`OK`

A response from the device after it processes the command to get app feedback from a managed app.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

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

        DeleteFeedback

        Identifiers

            com.acme.myenterpriseapp

        RequestType
        ManagedApplicationFeedback

    CommandUUID
    0001_ManagedApplicationFeedback

```

```

    CommandUUID
    0090_ManagedApplicationFeedback
    ManagedApplicationFeedback

            Feedback

                feedback
                Feedback

            Identifier
            com.acme.myenterpriseapp

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ManagedApplicationFeedbackCommand

The command to get managed app feedback on a device.

object ManagedApplicationFeedbackResponse

A response from the device after it processes the command to get app feedback from a managed app.

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

List the Managed Apps

Get the status of all managed apps on a device.

Query App Attributes

Query attributes in managed apps on a device.

Get App Configuration

Get app configurations from managed apps on a device.

