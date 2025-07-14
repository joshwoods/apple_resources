

- Device Management
-  SecurityIdentity 

Object

# SecurityIdentity

The declaration to install an identity on the device.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityIdentity
```

## Properties

`AllowAllAppsAccess`

`boolean`

If `true`, apps can access the private key.

Default: `false`

`CredentialAssetReference`

`string`

 (Required) 

The identifier of an asset declaration that contains the identity to install.

`KeyIsExtractable`

`boolean`

If `true`, the private key is extractable in the keychain.

Default: `true`

## Discussion

Specify `com.apple.configuration.security.identity` as the declaration type.

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

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

