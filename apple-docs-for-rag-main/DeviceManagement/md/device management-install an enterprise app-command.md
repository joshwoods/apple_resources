

- Device Management
-  Install an Enterprise App 

Web Service Endpoint

# Install an Enterprise App

Install an enterprise app on a device.

macOS 10.13.6+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InstallEnterpriseApplicationCommand
```

## HTTP Body

InstallEnterpriseApplicationCommand

The command to install an enterprise app on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InstallEnterpriseApplicationResponse

`OK`

A response from the device after it processes the command to install an enterprise app.

Content-Type: application/xml

## Discussion

This command provides a more secure version of `InstallApplication` that specifies a `ManifestURL`. The request must contain either `Manifest` or `ManifestURL`. Using `Manifest` ignores the pinning options. When using `ManifestURL`, specify the pinning options to increase security. In macOS, the device returns an `Acknowledged` response after validating the parameters, but before downloading and installing the app. Howevever, it doesn’t notify the MDM server about errors that occur during the installation process.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                             |
|----------------------------|-----------------------------|
| Device Channel             | macOS                       |
| User Channel               | \-                          |
| Requires Supervision       | \-                          |
| Allowed in User Enrollment | macOS                       |
| Required Access Right      | AllowPasscodeRemovalAndLock |

### Example Request and Response

- Request
- Response

```

    Command

        ManifestURL
        https://yourmdmhost.example.com/files/myenterpriseapp.plist
        PinningRevocationCheckRequired

        RequestType
        InstallEnterpriseApplication

    CommandUUID
    0001_InstallEnterpriseApplication

```

```

    CommandUUID
    0001_InstallEnterpriseApplication
    Queued

    Status
    Acknowledged
    UDID
    E84CD517-CB37-52F7-988C-DB5137B604B8

```

## Topics

### Command and Response

object InstallEnterpriseApplicationCommand

The command to install an enterprise app on a device.

object InstallEnterpriseApplicationResponse

A response from the device after it processes the command to install an enterprise app.

## See Also

### Managed Apps

Install an App

Install a third-party app on a device.

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

Get App Feedback

Get app feedback from a managed app on the device.

