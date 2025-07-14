

- Device Management
- SettingsCommand
- 
  - SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.PasscodeLockGracePeriod Deprecated

Device Management Command

# SettingsCommand.Command.Settings.PasscodeLockGracePeriod

A dictionary that contains settings for the password lock grace period.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.PasscodeLockGracePeriod
```

Deprecated

Use `PasscodeLockGracePeriod` in SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy instead.

## Properties

`Item`

`string`

Deprecated   (Required) 

A string that identifies this setting.

Value: `PasscodeLockGracePeriod`

`PasscodeLockGracePeriod`

`integer`

Deprecated   (Required) 

The number of seconds before a locked screen requires the user to enter the device passcode to unlock it. The minimum value is `0` seconds and the maximum value is `14400` seconds.

If a device has a passcode, a change to a larger value doesn’t take effect until the user logs out or removes the passcode. For this reason, it’s better to set this value before the user sets a passcode.

This setting won’t take effect if `TemporarySessionOnly` is `true` because there’s no passcode for a temporary session.

Possible Values: `0, 60, 300, 900, 3600, 14400`

## Discussion

This setting doesn’t support User Enrollment, and is only available on Shared iPad.

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

