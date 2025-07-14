

- Device Management
-  Schedule an OS Update 

Web Service Endpoint

# Schedule an OS Update

Schedule an update of the operating system on a device.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ScheduleOSUpdateCommand
```

## HTTP Body

ScheduleOSUpdateCommand

The command to schedule an update of the operating system.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ScheduleOSUpdateResponse

`OK`

A response from the device after it processes the command to schedule an update of the operating system.

Content-Type: application/xml

## Discussion

Only supervised iOS, macOS, and tvOS devices are eligible for software update management.

This command can only schedule operating-system updates in iOS and tvOS, however, it can also schedule a variety of system software updates in macOS.

Downloading and installing updates in iOS and tvOS is a two-step process. Send a `ScheduleOSUpdate` command with `Default` for `InstallAction` to download the updates. Then send another `ScheduleOSUpdate` command with a `Default` `InstallAction` to install the updates. Software updates may require a restart, which prevents the device from responding. When this happens, the MDM server resends the `ScheduleOSUpdate` command when the device checks in again, however, the device won’t return a value for `UpdateResults`.

This command uses the ScheduleOSUpdateCommand.Command.UpdatesItem `InstallAction` values to offer varying degrees of control to the user of a device. The user can control the update with the `NotifyOnly` and `DownloadOnly` actions, which don’t initiate the update process at all. The `InstallASAP` and `InstallForceRestart` actions attempt to install the update as soon as possible. On iOS devices with a passcode, the user must authorize the update by entering their passcode, allowing them to defer the update a limited number of times. After the user reaches that limit, the system prompts to update every time the device returns to the home screen. This makes the device virtually unusable until the user approves the software update. On macOS devices, the `InstallLater` action provides a similar behavior, which specifies how many times the user may defer the update before it’s forced.

A device may return a different `InstallAction` than requested.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | \-                            |
| Requires Supervision       | iOS, macOS, tvOS              |
| Allowed in User Enrollment | \-                            |
| Required Access Right      | AllowAppInstallation          |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ScheduleOSUpdate
        Updates

                InstallAction
                DownloadOnly
                ProductKey
                iOSUpdate17A576
                ProductVersion
                13.0

    CommandUUID
    0001_ScheduleOSUpdate

```

```

    CommandUUID
    0001_ScheduleOSUpdate
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E
    UpdateResults

            InstallAction
            DownloadOnly
            ProductKey
            iOSUpdate17A576
            Status
            Downloading

```

## Topics

### Command and Response

object ScheduleOSUpdateCommand

The command to schedule an update of the operating system.

object ScheduleOSUpdateResponse

A response from the device after it processes the command to schedule an update of the operating system.

## See Also

### Updates

Schedule an OS Update Scan

Schedule a background scan for operating-system updates on a device.

List the Available OS Updates

Get a list of available operating-system updates for a device.

Get the OS Update Status

Get the status of operating-system updates on a device.

