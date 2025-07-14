

- Device Management
- SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.Wallpaper 

Device Management Command

# SettingsCommand.Command.Settings.Wallpaper

A dictionary that contains wallpaper settings.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.Wallpaper
```

## Properties

`Image`

`data`

 (Required) 

A Base64-encoded image in either PNG or JPG format to use for wallpaper.

`Item`

`string`

 (Required) 

A string that identifies this setting.

Value: `Wallpaper`

`Where`

`integer`

 (Required) 

A number that indicates where to use the wallpaper, which is one of the following values:

- `1`: Lock screen

- `2`: Home screen

- `3`: Both lock and home screens.

  In iOS 16 and later, and iPadOS 17 and later, when you set the wallpaper for the first time, the system sets both the lock screen and home screen. After that, you can separately set each location.

Possible Values: `1, 2, 3`

## Discussion

This setting doesn’t support User Enrollment, and is available on supervised devices only in iOS 8 and later.

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

