

- Device Management
-  Get App Configuration 

Web Service Endpoint

# Get App Configuration

Get app configurations from managed apps on a device.

iOS 7.0+iPadOS 7.0+macOS 10.15+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ManagedApplicationConfigurationCommand
```

## HTTP Body

ManagedApplicationConfigurationCommand

The command to get managed app configurations on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ManagedApplicationConfigurationResponse

`OK`

A response from the device after it processes the command to get app configurations from managed apps.

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
| Required Access Right      | AllowAppInstallation                   |

### Example Request and Response

- Request
- Response

```

    Command

        Identifiers

            com.acme.myenterpriseapp

        RequestType
        ManagedApplicationConfiguration

    CommandUUID
    0001_ManagedApplicationConfiguration

```

```

    ApplicationConfigurations

            Configuration

                text
                myappsettings

            Identifier
            com.acme.myenterpriseapp

    CommandUUID
    0001_ManagedApplicationConfiguration
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ManagedApplicationConfigurationCommand

The command to get managed app configurations on a device.

object ManagedApplicationConfigurationResponse

A response from the device after it processes the command to get app configurations from managed apps.

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

Get App Feedback

Get app feedback from a managed app on the device.

