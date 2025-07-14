

- Device Management
- SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.ApplicationConfiguration 

Device Management Command

# SettingsCommand.Command.Settings.ApplicationConfiguration

A dictionary that contains the configurations to apply to the app.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.ApplicationConfiguration
```

## Properties

`Configuration`

SettingsCommand.Command.Settings.ApplicationConfiguration.Configuration

A dictionary that contains the configurations to apply to the app. Omit this setting to remove existing configurations.

`Identifier`

`string`

 (Required) 

The bundle identifier of the managed app.

Important

`Item`

`string`

 (Required) 

Value: `ApplicationConfiguration`

## Overview

Note

For a watchOS app, the identifier needs to be the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired. Obtain the watch’s bundle identifier for an app with a watch bundle, in the `watchBundleId` key that’s part of the Content Metadata query. For more information on this query, see Getting App and Book Information (Legacy).

- Item: A string that identifies this setting.

## Discussion

This setting requires the App Management access right, and is available in iOS 7 and later, macOS 10.15 and later, and tvOS 10.2 and later.

In macOS 10.15 and later, the device channel supports this setting for User Enrollment only, using any bundle identifier.

In macOS 11 and later, the device channel also supports this setting for User Enrollment.

## Topics

### Commands

object SettingsCommand.Command.Settings.ApplicationConfiguration.Configuration

A dictionary that contains the configurations to apply to the app.

## See Also

### Commands

object SettingsCommand.Command.Settings.AccessibilitySettings

A dictionary that contains settings for accessibility.

object SettingsCommand.Command.Settings.AppAnalytics

A dictionary that contains settings for sharing app analytics.

object SettingsCommand.Command.Settings.ApplicationAttributes

A dictionary that contains the attributes to apply to the app.

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

