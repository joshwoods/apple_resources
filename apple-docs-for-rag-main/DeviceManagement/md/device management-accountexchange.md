

- Device Management
-  AccountExchange 

Object

# AccountExchange

The declaration to configure an Exchange account.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountExchange
```

## Properties

`AuthenticationCredentialsAssetReference`

`string`

The identifier of an asset declaration that contains the credentials for this account to authenticate with an Exchange server. Set the corresponding asset type to `CredentialUserNameAndPassword`.

`AuthenticationIdentityAssetReference`

`string`

The identifier of a credential asset declaration that contains the identity that this account requires to authenticate with the Exchange server.

`CalendarServiceActive`

`boolean`

If `true`, activates the calendar service for this account.

Default: `true`

`ContactsServiceActive`

`boolean`

If `true`, activates the address book service for this account.

Default: `true`

`EnabledProtocolTypes`

`[string]`

 (Required) 

The set of protocol types to enable on the Exchange server, in order of preference. This is an array of unique strings with possible values:

- `EAS:` Exchange ActiveSync

- `EWS:` Exchange Web Services (EWS)

If the device supports one or more of the listed protocol types, it sets up an account for the first supported type.

If the device doesn’t support any of the listed protocol types, it doesn’t set up an account and the system reports an error.

Possible Values: `EAS, EWS`

`External Path`

`string`

The external path of the EWS server. The system uses this only when this declaration has a `HostName` value.

`ExternalHostName`

`string`

The external hostname of the EWS server (or IP address). This is a required field unless the declaration contains an `OAuth` property, with a `SignInURL` that has `enabled` as `true`.

`ExternalPort`

`integer`

The external port number of the EWS server. The system uses this only when this declaration has a `HostName` value.

`HostName`

`string`

The IP address or fully qualified domain name (FQDN) of the Exchange host. This is a required field unless the declaration contains an `OAuth` property, with a `SignInURL` that has `enabled` as `true`.

`LockCalendarService`

`boolean`

If `true`, the system prevents the user from changing the status of the calendar service for this account.

Default: `false`

`LockContactsService`

`boolean`

If `true`, the system prevents the user from changing the status of the address book service for this account.

Default: `false`

`LockMailService`

`boolean`

If `true`, the system prevents the user from changing the status of the mail service for this account.

Default: `false`

`LockNotesService`

`boolean`

If `true`, the system prevents the user from changing the status of the notes service for this account.

Default: `false`

`LockRemindersService`

`boolean`

If `true`, the system prevents the user from changing the status of the reminders service for this account.

Default: `false`

`MailServiceActive`

`boolean`

If `true`, the system activates the mail service for this account.

Default: `true`

`NotesServiceActive`

`boolean`

If `true`, the system activates the notes service for this account.

Default: `true`

`OAuth`

AccountExchangeOAuthObject

The configuration settings for OAuth for this account.

`Path`

`string`

The path of the EWS server. The system uses this only when this declaration has a `HostName` value.

`Port`

`integer`

The port number of the EWS server. The system uses this only when this declaration has a `HostName` value.

`RemindersServiceActive`

`boolean`

If `true`, the system activates the reminders service for this account.

Default: `true`

`SMIME`

AccountExchangeSMIMEObject

Settings for S/MIME.

`UserIdentityAssetReference`

`string`

The identifier of an asset declaration that contains the user identity for this account. The corresponding asset must be of type `UserIdentity`.

`VisibleName`

`string`

The name that apps show to the user for this Exchange account. If not present, the system generates a suitable default.

## Discussion

Specify `com.apple.configuration.account.exchange` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS         |
|------------------------------|--------------------|
| Allowed in User Enrollment   | iOS, macOS         |
| Allowed in Local Enrollment  | iOS, macOS         |
| Allowed in System Scope      | iOS                |
| Allowed in User Scope        | macOS, Shared iPad |

## Topics

### Supporting Objects

object AccountExchangeOAuthObject

The declaration for configuring OAuth authentication of an Exchange account.

object AccountExchangeSMIMEObject

Settings for S/MIME.

object AccountExchangeSMIME_EncryptionObject

Settings for S/MIME encryption.

object AccountExchangeSMIME_SigningObject

Settings for S/MIME signing.

## See Also

### Configurations

object AccountCalDAV

The declaration to configure a Calendar account.

object AccountCardDAV

The declaration to configure an address book account.

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

object SafariExtensionSettings

The declaration to configure Safari Extensions.

