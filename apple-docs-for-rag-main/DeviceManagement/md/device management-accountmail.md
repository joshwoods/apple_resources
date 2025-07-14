

- Device Management
-  AccountMail 

Object

# AccountMail

The declaration to configure a Mail account.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountMail
```

## Properties

`IncomingServer`

AccountMailIncomingServerObject

 (Required) 

The settings for the incoming mail server for this account.

`OutgoingServer`

AccountMailOutgoingServerObject

 (Required) 

The settings for the outgoing mail server for this account.

`SMIME`

AccountMailSMIMEObject

Settings for S/MIME.

`UserIdentityAssetReference`

`string`

The identifier of an asset declaration that contains the user identity for this account. Set the corresponding asset type to `UserIdentity`.

`VisibleName`

`string`

The name that apps show to the user for this mail account. If not present, the system generates a suitable default.

## Discussion

Specify `com.apple.configuration.account.mail` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS         |
|------------------------------|--------------------|
| Allowed in User Enrollment   | iOS, macOS         |
| Allowed in Local Enrollment  | iOS, macOS         |
| Allowed in System Scope      | iOS                |
| Allowed in User Scope        | macOS, Shared iPad |

## Topics

### Supporting Objects

object AccountMailIncomingServerObject

The settings for configuring an incoming mail server.

object AccountMailOutgoingServerObject

The settings for configuring an outgoing mail server.

object AccountMailSMIMEObject

Settings for S/MIME.

object AccountMailSMIME_EncryptionObject

Settings for S/MIME encryption.

object AccountMailSMIME_SigningObject

Settings for S/MIME signing.

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

object SafariExtensionSettings

The declaration to configure Safari Extensions.

