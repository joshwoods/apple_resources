

- Device Management
-  ServicesBackgroundTasks 

Object

# ServicesBackgroundTasks

The declaration to configure background tasks.

macOS 15.0+Device Assignment ServicesVPP License Management

``` source
object ServicesBackgroundTasks
```

## Properties

`ExecutableAssetReference`

`string`

Specifies the identifier of an asset declaration containing a reference to the files to be used for the background task configuration. The corresponding asset must be of type “`com.apple.asset.data`”.

The referenced data must be a zip archive of an entire directory, that will be expanded and stored in a well known location for the background task. The asset’s “ContentType” and “Hash-SHA-256” keys in the “Reference” key are required.

This file should contain background task executables, scripts, and configuration files, but not the `launchd` configuration files.

`LaunchdConfigurations`

`[`ServicesBackgroundTasksLaunchdItemObject`]`

An array of `launchd` configuration files used to run the background tasks.

`TaskDescription`

`string`

A description of the set of background tasks managed by this configuration.

`TaskType`

`string`

 (Required) 

The unique identifier of the set of background tasks managed with this configuration. This should be a reverse DNS style identifier. The system uses this identifier to differentiate between tasks in different configurations.

## Topics

### Supporting Objects

object ServicesBackgroundTasksLaunchdItemObject

A dictionary of launchd configurations.

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

