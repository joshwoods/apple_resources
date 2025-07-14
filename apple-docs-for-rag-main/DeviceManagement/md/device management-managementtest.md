

- Device Management
-  ManagementTest 

Object

# ManagementTest

The declaration to test the MDM system.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagementTest
```

## Properties

`Echo`

`string`

 (Required) 

The string to echo back in a status response reason.

`EchoDataAssetReference`

`string`

The string to read from a data asset to echo back in status response reason description.

`ReturnStatus`

`string`

The status the system reports back when the device implements the configuration. Use this to override the normal `success` result.

Default: `Installed`

Possible Values: `Installed, Failed, Unlocked`

## Discussion

Specify `com.apple.configuration.management.test` as the declaration type.

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

object LegacyProfile

The declaration to configure a legacy profile.

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

object SafariExtensionSettings

The declaration to configure Safari Extensions.

