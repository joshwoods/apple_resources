

- Device Management
- SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.AccessibilitySettings 

Device Management Command

# SettingsCommand.Command.Settings.AccessibilitySettings

A dictionary that contains settings for accessibility.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.AccessibilitySettings
```

## Properties

`BoldTextEnabled`

`boolean`

If `true`, the system enables bold text.

Default: `false`

`GrayscaleEnabled`

`boolean`

If `true`, the system enables grayscale display.

Default: `false`

`IncreaseContrastEnabled`

`boolean`

If `true`, the system enables increase contrast.

Default: `false`

`Item`

`string`

 (Required) 

Sets various accessibility settings. The system allows only keys with explicitly provided values.

Value: `AccessibilitySettings`

`ReduceMotionEnabled`

`boolean`

If `true`, the system enables reduced motion.

Default: `false`

`ReduceTransparencyEnabled`

`boolean`

If `true`, the system enables reduced transparency.

Default: `false`

`TextSize`

`integer`

The accessibility text size apps that support dynamic text use. `0` is the smallest value, and `11` is the largest available.

Default: `4`

Possible Values: `0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11`

`TouchAccommodationsEnabled`

`boolean`

If `true`, the system enables touch accommodations.

Default: `false`

`VoiceOverEnabled`

`boolean`

If `true`, the system enables voiceover.

Default: `false`

`ZoomEnabled`

`boolean`

If `true`, the system enables zoom.

Default: `false`

## See Also

### Commands

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

object SettingsCommand.Command.Settings.Wallpaper

A dictionary that contains wallpaper settings.

