

- Device Management
-  List the Installed Apps 

Web Service Endpoint

# List the Installed Apps

Get a list of the installed apps on a device.

iOS 5.0+iPadOS 5.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InstalledApplicationListCommand
```

## HTTP Body

InstalledApplicationListCommand

The command to get a list of installed apps on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InstalledApplicationListResponse

`OK`

A response from the device after it processes the command to get a list of installed apps.

Content-Type: application/xml

## Discussion

The response includes system apps on macOS devices, however, it doesn’t include them on iOS devices.

Refer to the following sections to determine supported channels and requirements, and to see request and response examples for iOS and macOS.

### Query Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS                                    |
| Required Access Right      | AllowQueryApplications                 |

### Example Request and Response in iOS

- Request
- Response

```

    Command

        ManagedAppsOnly

        RequestType
        InstalledApplicationList

    CommandUUID
    0001_InstalledApplicationList

```

```

    CommandUUID
    0001_InstalledApplicationList
    InstalledApplicationList

            AdHocCodeSigned

            AppStoreVendable

            BetaApp

            BundleSize
            1036288
            DeviceBasedVPP

            DynamicSize
            8192
            ExternalVersionIdentifier
            0
            Identifier
            com.acme.myenterpriseapp
            Installing

            IsValidated

            Name
            MyEnterpriseApp
            ShortVersion
            1.0
            Version
            1.0

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

### Example Request and Response in macOS

- Request
- Response

```

    Command

        ManagedAppsOnly

        RequestType
        InstalledApplicationList

    CommandUUID
    0001_InstalledApplicationList

```

```

    CommandUUID
    0001_InstalledApplicationList
    InstalledApplicationList

            BundleSize
            1
            Identifier
            com.apple.Safari
            Installing

            Name
            Safari
            ShortVersion
            13.1.2
            Version
            13.1.2

            BundleSize
            1
            Identifier
            com.apple.Notes
            Installing

            Name
            Notes
            ShortVersion
            4.7
            Version
            4.7

            BundleSize
            1
            Identifier
            com.apple.AddressBook
            Installing

            Name
            Contacts
            ShortVersion
            12.0
            Version
            12.0

            BundleSize
            1
            Identifier
            com.apple.mail
            Installing

            Name
            Mail
            ShortVersion
            13.4
            Version
            13.4

            BundleSize
            1
            Identifier
            com.apple.iCal
            Installing

            Name
            Calendar
            ShortVersion
            11.0
            Version
            11.0

    Status
    Acknowledged
    UDID
    91FE0F6E-F91C-589A-95E6-02835CE7126D

```

## Topics

### Command and Response

object InstalledApplicationListCommand

The command to get a list of installed apps on a device.

object InstalledApplicationListResponse

A response from the device after it processes the command to get a list of installed apps.

## See Also

### Device Details

Get Device Information

Get detailed information about a device.

Release Device from Await Configuration

Inform the device that it can allow the user to continue in Setup Assistant.

User Configured Command

Informs the device that it can continue past Setup Assistant and finish login.

List the Installed Restrictions

Get a list of restrictions on the device.

