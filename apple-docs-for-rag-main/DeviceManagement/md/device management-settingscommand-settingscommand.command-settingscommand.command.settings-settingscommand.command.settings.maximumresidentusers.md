

- Device Management
- SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.MaximumResidentUsers 

Device Management Command

# SettingsCommand.Command.Settings.MaximumResidentUsers

A dictionary that contains settings for maximum resident users.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.MaximumResidentUsers
```

## Properties

`Item`

`string`

Deprecated   (Required) 

A string that identifies this setting.

Value: `MaximumResidentUsers`

`MaximumResidentUsers`

`integer`

Deprecated   (Required) 

The maximum number of users that can use the device. If this value is greater than the value for the maximum possible number of users that the device suports, the MDM server uses that value instead.

This setting requires that the device is in the `AwaitingConfiguration` phase before it receives the DeviceConfigured message.

When a device reaches the maximum number of resident users and a new user tries to sign in, the MDM server removes a synchronized user to make space for the new user. If there are no synchronized users, the new user sign-in fails. A synchronized user is a user that has completed syncing their data.

## Discussion

Apple deprecated this setting in iOS 13.4. Use SettingsCommand.Command.Settings.SharedDeviceConfiguration instead. This setting doesn’t support User Enrollment, and is only available for Shared iPad.

## See Also

### Commands

object SettingsCommand.Command.Settings.AccessibilitySettings

A dictionary that contains settings for accessibility.

object SettingsCommand.Command.Settings.AppAnalytics

A dictionary that contains settings for sharing app analytics.

object SettingsCommand.Command.Settings.ApplicationAttributes

A dictionary that contains the attributes to apply to the app.

object SettingsCommand.Command.Settings.ApplicationConfiguration

A dictionary that contains the configurations to apply to the app.

object SettingsCommand.Command.Settings.Bluetooth

A dictionary that contains Bluetooth settings.

object SettingsCommand.Command.Settings.DataRoaming

A dictionary that contains data roaming settings.

object SettingsCommand.Command.Settings.DeviceName

A dictionary that contains device name settings.

object SettingsCommand.Command.Settings.DiagnosticSubmission

A dictionary that contains diagnostic submission settings.

object SettingsCommand.Command.Settings.HostName

A dictionary that contains hostname settings.

object SettingsCommand.Command.Settings.MDMOptions

A dictionary that contains settings about the organization operating the MDM server.

object SettingsCommand.Command.Settings.OrganizationInfo

A dictionary that contains settings about the organization operating the MDM server.

object SettingsCommand.Command.Settings.PersonalHotspot

A dictionary that contains Personal Hotspot settings.

object SettingsCommand.Command.Settings.SharedDeviceConfiguration

A dictionary that contains shared device configuration settings.

object SettingsCommand.Command.Settings.SoftwareUpdateSettings

A dictionary that contains software update settings.

object SettingsCommand.Command.Settings.TimeZone

A dictionary that contains time zone settings.

