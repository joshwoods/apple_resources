

- Device Management
-  AssociatedDomains 

Device Management Profile

# AssociatedDomains

The payload you use to configure associated domains.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object AssociatedDomains
```

## Properties

`Configuration`

`[`AssociatedDomains.ConfigurationItem`]`

 (Required) 

A dictionary that maps apps to their associated domains.

## Discussion

Specify `com.apple.associated-domains` as the payload type.

You can use associated domains with features such as Extensible AppSSO, universal links, and Password AutoFill.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            Configuration

                    ApplicationIdentifier
                    com.apple.mobilesafari
                    AssociatedDomains

                        www.example.com

            PayloadIdentifier
            com.example.myassociateddomainpayload
            PayloadType
            com.apple.associated-domains
            PayloadUUID
            7f6e26da-c381-4666-9dc6-50b4cd418652
            PayloadVersion
            1

    PayloadDisplayName
    Associated Domains
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2c8c95c4-fde5-4e90-9dea-f8e9ab633562
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object AssociatedDomains.ConfigurationItem

A dictionary that maps apps to their associated domains.

## See Also

### App Management

object AppLock

The payload you use to configure a device to run a single app.

object AutonomousSingleAppMode

The payload you use to configure Autonomous Single App mode.

object NSExtensionManagement

The payload you use to configure the extensions that the system allows or disallows to run on the device.

