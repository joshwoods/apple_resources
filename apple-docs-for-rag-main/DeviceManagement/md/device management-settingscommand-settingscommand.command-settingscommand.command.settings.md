

- Device Management
- SettingsCommand
- SettingsCommand.Command
-  SettingsCommand.Command.Settings 

Device Management Command

# SettingsCommand.Command.Settings

An array of dictionaries that contains the settings.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings
```

## Properties

`AccessibilitySettings`

SettingsCommand.Command.Settings.AccessibilitySettings

A dictionary that contains accessibility settings. Available in iOS 16 and later.

`AppAnalytics`

SettingsCommand.Command.Settings.AppAnalytics

A dictionary that contains settings for sharing app analytics. This setting doesn’t support User Enrollment, and is only available for Shared iPad. Available in iOS 9.3.2 and later.

`ApplicationAttributes`

SettingsCommand.Command.Settings.ApplicationAttributes

A dictionary that contains the attributes to apply to the app. Omit this setting to remove existing attributes. This setting supports User Enrollment, is available in iOS 7 and later, and tvOS 10.2 and later.

`ApplicationConfiguration`

SettingsCommand.Command.Settings.ApplicationConfiguration

A dictionary that contains the configurations to apply to the app. Omit this setting to remove existing configurations. This setting requires the App Management access right, supports User Enrollment, and is available in iOS 7 and later, macOS 10.15 and later, and tvOS 10.2 and later.

`Bluetooth`

SettingsCommand.Command.Settings.Bluetooth

A dictionary that contains Bluetooth settings. This setting requires the Network Information access right, doesn’t support User Enrollment, is only available on supervised devices, and is available in iOS 11.3 and later, and macOS 10.13.4 and later.

`DataRoaming`

SettingsCommand.Command.Settings.DataRoaming

A dictionary that contains data roaming settings. This setting requires the Network Information access right, doesn’t support User Enrollment, and is available in iOS 5 and later.

`DeviceName`

SettingsCommand.Command.Settings.DeviceName

A dictionary that contains device name settings. This setting doesn’t support User Enrollment, and is only available on supervised devices. Available on iOS 5 and later.

`DiagnosticSubmission`

SettingsCommand.Command.Settings.DiagnosticSubmission

A dictionary that contains diagnostic submission settings. This setting doesn’t support User Enrollment, and is only available for Shared iPad. Available in iOS 9.3 and later.

`HostName`

SettingsCommand.Command.Settings.HostName

A dictionary that contains hostname settings. This setting doesn’t support User Enrollment, and is available in macOS 10.11 and later.

`MaximumResidentUsers`

SettingsCommand.Command.Settings.MaximumResidentUsers

Deprecated 

A dictionary that contains settings for maximum resident users. Apple deprecated this setting in iOS 13.4. Use `SharedDeviceConfiguration` instead. This setting doesn’t support User Enrollment, and is only available for Shared iPad.

`MDMOptions`

SettingsCommand.Command.Settings.MDMOptions

A dictionary that contains settings related to the MDM protocol. This setting doesn’t support User Enrollment, and is available in iOS 7 and later, and macOS 10.15 and later.

`OrganizationInfo`

SettingsCommand.Command.Settings.OrganizationInfo

A dictionary that contains settings about the organization operating the MDM server. This setting supports User Enrollment. Available in iOS 5 and later.

`PersonalHotspot`

SettingsCommand.Command.Settings.PersonalHotspot

A dictionary that contains Personal Hotspot settings. This setting requires the Network Information access right, doesn’t support User Enrollment, and is available in iOS 5 and later.

`SharedDeviceConfiguration`

SettingsCommand.Command.Settings.SharedDeviceConfiguration

A dictionary that contains shared device configuration settings. This setting doesn’t support User Enrollment, and is available in iOS 13.4 and later for Shared iPad.

`SoftwareUpdateSettings`

SettingsCommand.Command.Settings.SoftwareUpdateSettings

A dictionary that contains software update settings. This setting doesn’t support User Enrollment, and is available in iOS 14.5 and later.

`TimeZone`

SettingsCommand.Command.Settings.TimeZone

A dictionary that contains time zone settings. This setting is only available on supervised devices and doesn’t support User Enrollment. Available in iOS 14 and later, and tvOS 14 and later.

`Wallpaper`

SettingsCommand.Command.Settings.Wallpaper

A dictionary that contains wallpaper settings. This setting doesn’t support User Enrollment, and is available in iOS 8 and later.

`PasscodeLockGracePeriod`

SettingsCommand.Command.Settings.PasscodeLockGracePeriod

Deprecated 

A dictionary that contains password lock grace period settings. This setting doesn’t support User Enrollment, and is only available for Shared iPad. Available in iOS 9.3.2 and later.

This key is deprecated. Use `PasscodeLockGracePeriod` in SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy instead.

`VoiceRoaming`

SettingsCommand.Command.Settings.VoiceRoaming

Deprecated 

A dictionary that contains voice roaming settings. This setting requires the Network Information access right, doesn’t support User Enrollment, and is available in iOS 5 and later.

`DefaultApplications`

SettingsCommand.Command.Settings.DefaultApplications

## Topics

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

object SettingsCommand.Command.Settings.Wallpaper

A dictionary that contains wallpaper settings.

object SettingsCommand.Command.Settings.MaximumResidentUsers

A dictionary that contains settings for maximum resident users.

object SettingsCommand.Command.Settings.PasscodeLockGracePeriod

A dictionary that contains settings for the password lock grace period.

Deprecated

object SettingsCommand.Command.Settings.VoiceRoaming

A dictionary that contains voice roaming settings.

object SettingsCommand.Command.Settings.DefaultApplications

