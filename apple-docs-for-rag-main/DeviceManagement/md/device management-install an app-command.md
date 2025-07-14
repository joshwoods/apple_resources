

- Device Management
-  Install an App 

Web Service Endpoint

# Install an App

Install a third-party app on a device.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InstallApplicationCommand
```

## HTTP Body

InstallApplicationCommand

The command to install an app on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InstallApplicationResponse

`OK`

A response from the device after it processes the command to install a third-party app.

Content-Type: application/xml

## Discussion

If the app is a managed app, this command updates it. The request must contain only one of these keys: `iTunesStoreID`, `Identifier`, or `ManifestURL`.

Installation prompts the user to approve or cancel the update. If the device is supervised, the device only prompts when the app to install is in the foreground.

Set the organization name that appears in this prompt in the `OrganizationInfo` dictionary using the `Settings` command.

In macOS, the device returns an `Acknowledged` response after validating the parameters, but before downloading and installing the app. However, it doesn’t notify the MDM server about errors that occur during the installation process.

For macOS VPP app installations, if the app is device licensed, the system must receive the `InstallApplication` command on the device channel. If the app is user licensed, the system must receive the `InstallApplication` command on the user channel.

Prior to iOS 16.0 and tvOS 16.0, this command would return `NotNow` when Setup Assistant was running. Starting in iOS 16.0 and tvOS 16.0, the command may be sent to supervised devices during Setup Assistant. However, you should only attempt to install device-based VPP apps or enterprise apps while in the awaiting configuration state, as it is unlikely the device would have an App Store account configured, and thus commands that depend on one will fail.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowAppInstallation                   |

### Example Request and Response (Enterprise App)

- Request
- Response

```

    Command

        ManagementFlags
        0
        ManifestURL
        https://yourmdmhost.example.com/files/myenterpriseapp.plist
        RequestType
        InstallApplication

    CommandUUID
    0001_InstallApplication

```

```

    CommandUUID
    0001_InstallApplication
    Identifier
    com.acme.myenterpriseapp
    State
    Installing
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

### Example Request and Response (VPP App)

- Request
- Response

```

    Command

        ManagementFlags
        0
        Options

            PurchaseMethod
            1

        RequestType
        InstallApplication
        iTunesStoreID
        1096834193

    CommandUUID
    0001_InstallApplication

```

```

    CommandUUID
    0001_InstallApplication
    Identifier
    com.apple.TVRemote
    State
    Installing
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object InstallApplicationCommand

The command to install an app on a device.

object InstallApplicationResponse

A response from the device after it processes the command to install a third-party app.

## See Also

### Managed Apps

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

Get App Feedback

Get app feedback from a managed app on the device.

