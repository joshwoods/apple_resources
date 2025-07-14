

- Device Management
-  ServicesConfigurationFiles 

Object

# ServicesConfigurationFiles

The managed configuration files for services.

macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ServicesConfigurationFiles
```

## Properties

`DataAssetReference`

`string`

 (Required) 

The identifier of an asset declaration that contains a reference to the files to use for system service configuration. Ensure that the corresponding asset:

- Is of type `com.apple.asset.data`

- Is a zip archive of an entire directory

- Has a `Reference` key that includes the `ContentType` and `Hash-SHA-256` keys, which the system requires

The system expands the zip archive and stores the data in a well-known location for the service.

`ServiceType`

`string`

 (Required) 

The identifier of the system service with managed configuration files. Use a reverse DNS style for this identifier. However, the system reserves `com.apple.` prefix for built-in services. The available built-in services are:

- `com.apple.sshd` configures sshd

- `com.apple.sudo` configures sudo

- `com.apple.pam` configures PAM

- `com.apple.cups` configures CUPS

- `com.apple.apache.httpd` configures Apache httpd

- `com.apple.bash` configures bash

- `com.apple.zsh` configures zsh

## Discussion

Specify `com.apple.configuration.services.configuration-files` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | macOS |
|------------------------------|-------|
| Allowed in User Enrollment   | \-    |
| Allowed in Local Enrollment  | \-    |
| Allowed in System Scope      | macOS |
| Allowed in User Scope        | \-    |

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

