

- Device Management
- SettingsCommand
- 
  - SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
- SettingsCommand.Command.Settings.SharedDeviceConfiguration
-  SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy 

Device Management Command

# SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy

A dictionary that contains passcode policies.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy
```

## Properties

`AutoLockTime`

`integer`

The number of seconds before a device goes to sleep after being idle. The minimum value for this setting is `120` seconds.

`PasscodeLockGracePeriod`

`integer`

The number of seconds before a locked screen requires the user to enter the device passcode to unlock it. The minimum value is `0` seconds and the maximum value is `14400` seconds.

If a device has a passcode, a change to a larger value doesn’t take effect until the user logs out or removes the passcode. For this reason, it’s better to set this value before the user sets a passcode.

This setting won’t take effect if `TemporarySessionOnly` is `true` because there’s no passcode for a temporary session.

Possible Values: `0, 60, 300, 900, 3600, 14400`

## Discussion

This setting is only available on Shared iPad on iPadOS 17 and later.

## See Also

### Commands

object SettingsCommand.Command.Settings.SharedDeviceConfiguration.AwaitUserConfiguration

Enables the user configuration Setup Assistant workflow.

