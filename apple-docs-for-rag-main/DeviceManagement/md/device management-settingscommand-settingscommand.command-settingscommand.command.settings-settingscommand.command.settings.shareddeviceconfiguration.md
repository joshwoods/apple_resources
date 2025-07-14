

- Device Management
- SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
-  SettingsCommand.Command.Settings.SharedDeviceConfiguration 

Device Management Command

# SettingsCommand.Command.Settings.SharedDeviceConfiguration

A dictionary that contains shared device configuration settings.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.SharedDeviceConfiguration
```

## Properties

`AwaitUserConfiguration`

SettingsCommand.Command.Settings.SharedDeviceConfiguration.AwaitUserConfiguration

If enabled, the Shared iPad device enters Setup Assistant after the user triggers a login. The MDM server has a chance to configure the device and user. After configuration, a UserConfiguredCommand needs be sent to the user channel to unblock the login. This feature requires the device to have network access during the login process.

Available in iOS 17 and later.

`Item`

`string`

 (Required) 

A string that identifies this setting.

Value: `SharedDeviceConfiguration`

`ManagedAppleIDDefaultDomains`

`[string]`

A list of domains that the Shared iPad login screen displays. The user can pick a domain from the list to complete their Managed Apple ID.

If this list contains more than 3 domains, the system picks 3 at random for display. Available in iOS 16 and later.

`OnlineAuthenticationGracePeriod`

`integer`

A grace period (in days) for Shared iPad online authentication. The Shared iPad only verifies the user’s passcode locally during login for users that already exist on the device. However, the system requires an online authentication (against Apple’s identity server) after the number of days specified by this setting.

Setting this value to 0 enforces online authentication every time.

Available in iOS 16 and later.

`PasscodePolicy`

SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy

A dictionary that contains passcode policies.

`QuotaSize`

`integer`

The quota size, in megabytes (MB), for each user on the shared device, or if the quota size is too small, the minimum quota size. Available to Temporary Sessions Only guest users on iOS 17+.

`ResidentUsers`

`integer`

The expected number of users. If this value is greater than the value for the maximum possible number of users that the device supports, the MDM server uses that value instead.

`SkipLanguageAndLocaleSetupForNewUsers`

`boolean`

If `true`, the system picks the system language and locale automatically for the new Shared iPad user.

Available in iOS 16.2 and later.

Default: `false`

`TemporarySessionOnly`

`boolean`

If `true`, the user only sees the Guest Welcome pane and can only log in as a guest user.

If `false`, the user can sign in with a managed Apple ID (the existing behavior).

Available in iOS 14.5 and later.

Default: `false`

`TemporarySessionTimeout`

`integer`

The timeout, in seconds, for the temporary session. The temporary session logs out automatically after the specified period of inactivity. The minimum value is 30 seconds. Setting this value to `0` removes the timeout.

Available in iOS 14.5 and later.

`UserSessionTimeout`

`integer`

The timeout, in seconds, for the user session. The user session logs out automatically after the specified period of inactivity. The minimum value is 30 seconds. Setting this value to `0` removes the timeout.

Available in iOS 14.5 and later.

## Discussion

This setting doesn’t support user enrollment, and is available in iOS 13.4 and later for Shared iPad.

Apply this setting before users log in to the device. If you upgraded the device to iOS 13.4 or later, perform an erase of all content and settings before applying this setting. Provide either the `QuotaSize` or `ResidentUsers`. If you provide both values, the MDM server uses `QuotaSize`.

## Topics

### Commands

object SettingsCommand.Command.Settings.SharedDeviceConfiguration.AwaitUserConfiguration

Enables the user configuration Setup Assistant workflow.

object SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy

A dictionary that contains passcode policies.

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

object SettingsCommand.Command.Settings.SoftwareUpdateSettings

A dictionary that contains software update settings.

object SettingsCommand.Command.Settings.TimeZone

A dictionary that contains time zone settings.

object SettingsCommand.Command.Settings.Wallpaper

A dictionary that contains wallpaper settings.

