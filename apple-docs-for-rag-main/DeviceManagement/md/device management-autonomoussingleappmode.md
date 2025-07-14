

- Device Management
-  AutonomousSingleAppMode 

Device Management Profile

# AutonomousSingleAppMode

The payload you use to configure Autonomous Single App mode.

macOS 10.13.4+Device Assignment ServicesVPP License Management

``` source
object AutonomousSingleAppMode
```

## Properties

`AllowedApplications`

`[`AutonomousSingleAppMode.AllowedApplicationsItem`]`

 (Required) 

An array of dictionaries that specifies the apps that the system grants access to the Accessibility APIs.

## Discussion

Specify `com.apple.asam` as the payload type.

The system only allows installation of one profile of this type, and it requires installation through a user-approved MDM server. Apps listed in this profile have low-level access to the system, including, but not limited to, key logging and user interface manipulation outside the app’s context.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | \-    |
| Requires Supervision       | \-    |
| Requires User Approved MDM | macOS |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            AllowedApplications

                    BundleIdentifier
                    com.apple.safari
                    TeamIdentifier
                    team-id

            PayloadIdentifier
            com.example.myasampayload
            PayloadType
            com.apple.asam
            PayloadUUID
            c324fd3e-d98a-4ea8-818a-5991024cddd0
            PayloadVersion
            1

    PayloadDisplayName
    Autonomous Single App Mode
    PayloadIdentifier
    com.example.profile
    PayloadType
    Configuration
    PayloadUUID
    467ab3a0-9423-4c16-a05c-5c99d771088f
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object AutonomousSingleAppMode.AllowedApplicationsItem

A dictionary that specifies an app that can be granted access to the Accessibilty APIs.

## See Also

### App Management

object AppLock

The payload you use to configure a device to run a single app.

object AssociatedDomains

The payload you use to configure associated domains.

object NSExtensionManagement

The payload you use to configure the extensions that the system allows or disallows to run on the device.

