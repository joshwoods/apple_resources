

- Device Management
-  SoftwareUpdateSettings 

Object

# SoftwareUpdateSettings

The declaration to configure software updates.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdateSettings
```

## Properties

`AllowStandardUserOSUpdates`

`boolean`

If set to `true`, a standard user can perform Major and Minor Software Updates.

If set to `false`, only administrators can perform Major and Minor Software Updates.

Default: `true`

`AutomaticActions`

SoftwareUpdateSettingsAutomaticActionsObject

This object configures various automatic Software Update functionality.

`Beta`

SoftwareUpdateSettingsBetaObject

This object configures the beta program settings for a device.

`Deferrals`

SoftwareUpdateSettingsDeferralsObject

This object configures the deferral of software updates. Rapid Security Responses aren’t considered within ‘Major’, ‘Minor’, or ‘System’ deferral mechanism.

`Notifications`

`boolean`

If set to `true`, the device shows all software update enforcement notifications.

If set to `false`, the device only shows notifications triggered one hour before the enforcement deadline, and the restart countdown notification.

Default: `true`

`RapidSecurityResponse`

SoftwareUpdateSettingsRapidSecurityResponseObject

These configurations set user access to interacting with Rapid Security Responses (RSRs).

`RecommendedCadence`

`string`

This string specifies how the device shows software updates to the user. When more than one update is available update, the device behaves as follows:

- `All` - Shows all software update versions.

- `Oldest` - Shows only the oldest (lower numbered) software update version.

- `Newest` - Shows only the newest (highest numbered) software update version.

Possible Values: `All, Oldest, Newest`

## Topics

### Supporting Objects

object SoftwareUpdateSettingsAutomaticActionsObject

The object that configures various automatic Software Update functionality.

object SoftwareUpdateSettingsBetaObject

The object that configures overall beta program settings.

object SoftwareUpdateSettingsBeta_ProgramObject

The object that configures a specific beta program.

object SoftwareUpdateSettingsBeta_RequireProgramObject

The object that configures beta program requirement settings.

object SoftwareUpdateSettingsDeferralsObject

The object that configures update deferrals.

object SoftwareUpdateSettingsRapidSecurityResponseObject

The object that configures rapid security update settings.

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

