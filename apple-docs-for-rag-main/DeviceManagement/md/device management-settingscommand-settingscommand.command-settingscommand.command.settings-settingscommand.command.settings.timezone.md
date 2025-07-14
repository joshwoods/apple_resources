

- Device Management
- SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.TimeZone 

Device Management Command

# SettingsCommand.Command.Settings.TimeZone

A dictionary that contains time zone settings.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.TimeZone
```

## Properties

`Item`

`string`

 (Required) 

A string that identifies this setting.

Value: `TimeZone`

`TimeZone`

`string`

 (Required) 

The Internet Assigned Numbers Authority (IANA) time zone database name.

If the `forceAutomaticDateAndTime` restriction is set in Restrictions, this setting fails with an error. Otherwise, setting this value disables automatic time zone logic. The user is still be able to change the timezone; for example, by turning automatic date and time back on. The intention is to allow setting the timezone when automatic determination isn’t be available, such as when Location Services are off.

## Discussion

This setting is only supported on supervised devices and doesn’t support User Enrollment. This setting is available in iOS 14 and later, and tvOS 14 and later.

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

object SettingsCommand.Command.Settings.Wallpaper

A dictionary that contains wallpaper settings.

