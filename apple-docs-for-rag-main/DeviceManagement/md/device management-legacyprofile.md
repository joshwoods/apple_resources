

- Device Management
-  LegacyProfile 

Object

# LegacyProfile

The declaration to configure a legacy profile.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object LegacyProfile
```

## Properties

`ProfileURL`

`string`

 (Required) 

The URL of the profile to download and install, which needs to start with `https://`. The system silently ignores any account or passcode payloads in the profile. Use their declarative configurations instead.

If a user enrollment triggers this configuration, the system silently ignores any MDM 1 payloads in macOS where the User Enrollment Mode setting is `forbidden`. In iOS, the system rejects the entire profile.

## Discussion

Specify `com.apple.configuration.legacy` as the declaration type.

This declaration specifies an MDM 1 profile for the device to download and install.

The declaration may contain any profile that MDM supports. The system doesn’t allow MDM enrollment and Profile Services profiles.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS, tvOS, watchOS              |
|------------------------------|----------------------------------------|
| Allowed in User Enrollment   | iOS, macOS                             |
| Allowed in Local Enrollment  | iOS, macOS, tvOS, watchOS              |
| Allowed in System Scope      | iOS, macOS, Shared iPad, tvOS, watchOS |
| Allowed in User Scope        | macOS, Shared iPad                     |

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

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

object SafariExtensionSettings

The declaration to configure Safari Extensions.

