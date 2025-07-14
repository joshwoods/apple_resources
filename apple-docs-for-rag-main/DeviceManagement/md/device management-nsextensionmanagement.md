

- Device Management
-  NSExtensionManagement 

Device Management Profile

# NSExtensionManagement

The payload you use to configure the extensions that the system allows or disallows to run on the device.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object NSExtensionManagement
```

## Properties

`AllowedExtensions`

`[string]`

An array of bundle identifiers for allowed extensions.

`DeniedExtensionPoints`

`[string]`

An array of extension points for extensions that the system doesn’t allow to run.

`DeniedExtensions`

`[string]`

An array of bundle identifiers for extensions that the system doesn’t allow to run.

## Discussion

Specify `com.apple.NSExtension` as the payload type.

You can manage extensions by bundle identifiers in allow and deny lists, or by a deny list of extension points.

You can also start with all public extensions disallowed. To do so, include `AllPublicExtensionPoints` in `DeniedExtensionPoints`. This causes the system to expand the list to include all extensions that belong to any public extension points. This expansion occurs at evaluation time. The list of extension points can change from release to release. The expanded list disallows Apple and third-party extensions, but still allows extensions that belong to system-critcial extension points to execute.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            AllowedExtensions

                com.apple.share.AirDrop.send

            DeniedExtensions

                com.apple.ncplugin.stocks

            DeniedExtensionPoints

                com.apple.share-services

            PayloadIdentifier
            com.example.mynsempayload
            PayloadType
            com.apple.nsextension
            PayloadUUID
            9726bc46-1e51-466b-99e3-81b23561cf81
            PayloadVersion
            1

    PayloadDisplayName
    NS Extension Management
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    4cc87081-feee-46d1-b5d1-2a2fde9a8402
    PayloadVersion
    1

```

## See Also

### App Management

object AppLock

The payload you use to configure a device to run a single app.

object AssociatedDomains

The payload you use to configure associated domains.

object AutonomousSingleAppMode

The payload you use to configure Autonomous Single App mode.

