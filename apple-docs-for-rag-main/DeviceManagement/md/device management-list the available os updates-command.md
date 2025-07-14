

- Device Management
-  List the Available OS Updates 

Web Service Endpoint

# List the Available OS Updates

Get a list of available operating-system updates for a device.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#AvailableOSUpdatesCommand
```

## HTTP Body

AvailableOSUpdatesCommand

The command to get a list of available operating-system updates.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

AvailableOSUpdatesResponse

`OK`

A response from the device after it processes the command to get a list of available operating-system updates.

Content-Type: application/xml

## Discussion

This command is also available to execute on managed devices that aren’t enrolled in the Device Enrollment Program (DEP). A device must have a total of `DownloadSize` + `InstallSize` bytes available to successfully install a software update. In macOS, execute the `ScheduleOSUpdateScan` command to update the results that this command returns. In iOS and tvOS, the list only contains the latest available updates.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | \-                            |
| Requires Supervision       | iOS, tvOS                     |
| Allowed in User Enrollment | \-                            |
| Required Access Right      | AllowAppInstallation          |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        AvailableOSUpdates

    CommandUUID
    0001_AvailableOSUpdates

```

```

    AvailableOSUpdates

            AllowsInstallLater

            Build
            17A576
            DownloadSize
            251607570
            HumanReadableName
            iOS 13.0
            InstallSize
            1809842176
            IsCritical

            ProductKey
            iOSUpdate17A576
            ProductName
            iOS
            RestartRequired

            Version
            13.0

    CommandUUID
    0001_AvailableOSUpdates
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object AvailableOSUpdatesCommand

The command to get a list of available operating-system updates.

object AvailableOSUpdatesResponse

A response from the device after it processes the command to get a list of available operating-system updates.

## See Also

### Updates

Schedule an OS Update Scan

Schedule a background scan for operating-system updates on a device.

Schedule an OS Update

Schedule an update of the operating system on a device.

Get the OS Update Status

Get the status of operating-system updates on a device.

