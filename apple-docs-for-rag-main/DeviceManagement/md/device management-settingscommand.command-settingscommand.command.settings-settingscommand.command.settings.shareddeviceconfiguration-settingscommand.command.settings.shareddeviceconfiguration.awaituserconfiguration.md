

- Device Management
- SettingsCommand
- 
  - SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
- SettingsCommand.Command.Settings.SharedDeviceConfiguration
-  SettingsCommand.Command.Settings.SharedDeviceConfiguration.AwaitUserConfiguration 

Device Management Command

# SettingsCommand.Command.Settings.SharedDeviceConfiguration.AwaitUserConfiguration

Enables the user configuration Setup Assistant workflow.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.SharedDeviceConfiguration.AwaitUserConfiguration
```

## Properties

`Enabled`

`boolean`

 (Required) 

If `true`, the device stops at a Setup Assistant pane after user login. The user won’t be able to use the device until the device receives a UserConfiguredCommand command.

## See Also

### Commands

object SettingsCommand.Command.Settings.SharedDeviceConfiguration.PasscodePolicy

A dictionary that contains passcode policies.

