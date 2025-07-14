

- Device Management
-  AppLock 

Device Management Profile

# AppLock

The payload you use to configure a device to run a single app.

iOS 6.0+iPadOS 6.0+tvOS 10.2+Device Assignment ServicesVPP License Management

``` source
object AppLock
```

## Properties

`App`

AppLock.App

 (Required) 

A dictionary that contains information about the app.

## Discussion

Specify `com.apple.app.lock` as the payload type.

With an app lock profile, the device locks to the specified app until removal of the profile. The home button is in a disabled state, and the device returns to the app automatically upon wake or restart.

Only use an app lock payload after installing the target app.

### Profile Availability

|                            |                        |
|----------------------------|------------------------|
| Device Channel             | iOS, Shared iPad, tvOS |
| User Channel               | \-                     |
| Allow Manual Install       | \-                     |
| Requires Supervision       | iOS, tvOS              |
| Requires User Approved MDM | \-                     |
| Allowed in User Enrollment | \-                     |
| Allow Multiple Payloads    | \-                     |

### Profile Example

```

    PayloadContent

            App

                Identifier
                com.apple.mobilenotes

            PayloadIdentifier
            com.example.myapplockpayload
            PayloadType
            com.apple.app.lock
            PayloadUUID
            dc0c6fdd-aae0-4fd0-a19c-861ba28f4c55
            PayloadVersion
            1

    PayloadDisplayName
    Single App Mode
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    736f867e-3972-4889-aa68-7ce5be12eff6
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object AppLock.App

The only app available for use on the iOS device.

## See Also

### App Management

object AssociatedDomains

The payload you use to configure associated domains.

object AutonomousSingleAppMode

The payload you use to configure Autonomous Single App mode.

object NSExtensionManagement

The payload you use to configure the extensions that the system allows or disallows to run on the device.

