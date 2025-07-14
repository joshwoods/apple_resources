

- Device Management
-  SoftwareUpdateEnforcementSpecific 

Object

# SoftwareUpdateEnforcementSpecific

A software update enforcement policy for a specific OS release.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdateEnforcementSpecific
```

## Properties

`DetailsURL`

`string`

The URL of a web page that shows details that the organization provides about the enforced update.

`TargetBuildVersion`

`string`

The target build version to update the device to by the appropriate time, for example, `20A242`. The system uses the build version for testing during seeding periods. The build version can include a supplemental version identifier, for example, `20A242a`. If the build version isn’t consistent with the target OS version specified in the `TargetOSVersion` key, the target OS version takes precedence.

`TargetLocalDateTime`

`string`

 (Required) 

The local date time value that specifies when to force install the software update. Use the format `yyyy-mm-ddThh:mm:ss`, which is derived from RFC3339 but doesn’t include a time zone offset. If the user doesn’t trigger the software update before this time, the device force installs it.

`TargetOSVersion`

`string`

 (Required) 

The target OS version to update the device to by the appropriate time. This is the OS version number, for example, `16.1`. It may also include a supplemental version identifier, for example, `16.1.1`.

## Discussion

Specify `com.apple.configuration.softwareupdate.enforcement.specific` as the declaration type.

If the `TargetVersion` is an OS version that includes both a minor and patch version, then the system installs that specific version, for example, `16.1.1`. If the minor version doesn’t include a patch version, the system installs the latest available patch version. For example, if the `TargetVersion` is `16.1` and a `.1` patch is available, the system installs `16.1.1`.

The system can only install a supplemental software update on a device that already has the base OS version installed. For example, the system can only install a `16.1`(a) update on a device that currently has `16.1` installed, but it can’t install that update on a device that only has `16.0` installed. To update to a supplemental version from an older base version, use two configurations. Use the first configuration to update to the new base version, and the second configuration to update the new base version to its supplemental version.

If the device isn’t running at the target date-time, the system enforces the update one hour after restarting, or when the device meets all required conditions, such as minimum battery level.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS              |
|------------------------------|-------------------------|
| Allowed in User Enrollment   | \-                      |
| Allowed in Local Enrollment  | \-                      |
| Allowed in System Scope      | iOS, macOS, Shared iPad |
| Allowed in User Scope        | \-                      |

## See Also

### Configurations

object AccountCalDAV

The declaration to configure a Calendar account.

object AccountCardDAV

The declaration to configure an address book account.

object AccountExchange

The declaration to configure an Exchange account.

object AccountGoogle

The declaration to configure a Google account.

object AccountLDAP

The declaration to configure a Lightweight Directory Access Protocol (LDAP) account.

object AccountMail

The declaration to configure a Mail account.

object AccountSubscribedCalendar

The declaration to configure a Calendar subscription.

object AppManaged

The declaration to configure a managed app.

object DiskManagementSettings

The declaration to configure disk management settings on the device.

object LegacyInteractiveProfile

The declaration to configure an interactive, legacy profile.

object LegacyProfile

The declaration to configure a legacy profile.

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

