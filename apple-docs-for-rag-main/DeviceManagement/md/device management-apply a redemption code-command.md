

- Device Management
-  Apply a Redemption Code 

Web Service Endpoint

# Apply a Redemption Code

Complete the installation of an app using a redemption code.

iOS 5.0+iPadOS 5.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ApplyRedemptionCodeCommand
```

## HTTP Body

ApplyRedemptionCodeCommand

The command to send a redemption code to complete installation of an app on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ApplyRedemptionCodeResponse

`OK`

A response from the device after it processes the command to complete the installation of an app using a redemption code.

Content-Type: application/xml

## Discussion

Sending a redemption code to an app that doesn’t need it produces an error.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                      |
|----------------------------|----------------------|
| Device Channel             | iOS                  |
| User Channel               | \-                   |
| Requires Supervision       | \-                   |
| Allowed in User Enrollment | \-                   |
| Required Access Right      | AllowAppInstallation |

### Example Request and Response

- Request
- Response

```

    Command

        Identifier
        com.example.app
        RedemptionCode
        SB56LT7YX8RH
        RequestType
        ApplyRedemptionCode

    CommandUUID
    0001_ApplyRedemptionCode

```

```

    CommandUUID
    0001_ApplyRedemptionCode
    Status
    Acknowledged
    UDID
    00008020-001305842600013A

```

## Topics

### Command and Response

object ApplyRedemptionCodeCommand

The command to send a redemption code to complete installation of an app on a device.

object ApplyRedemptionCodeResponse

A response from the device after it processes the command to complete the installation of an app using a redemption code.

## See Also

### Managed Apps

Install an App

Install a third-party app on a device.

Install an Enterprise App

Install an enterprise app on a device.

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

Get App Feedback

Get app feedback from a managed app on the device.

