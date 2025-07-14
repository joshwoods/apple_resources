

- Device Management
- SettingsCommand
- 
  - SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
- SettingsCommand.Command.Settings.MDMOptions
-  SettingsCommand.Command.Settings.MDMOptions.MDMOptions 

Device Management Command

# SettingsCommand.Command.Settings.MDMOptions.MDMOptions

A dictionary that contains MDM options.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.MDMOptions.MDMOptions
```

## Properties

`ActivationLockAllowedWhileSupervised`

`boolean`

If `true`, a supervised device registers itself with Activation Lock when the user enables Find My. This setting is available for supervised devices in iOS 7 and later, and macOS 10.15 and later.

Default: `false`

`BootstrapTokenAllowed`

`boolean`

Deprecated 

If `true`, the server supports the Bootstrap Token commands.

Default: `false`

`IdleRebootAllowed`

`boolean`

Default: `false`

`PromptUserToAllowBootstrapTokenForAuthentication`

`boolean`

If `true`, warn the user that they need to reboot into RecoveryOS and allow the MDM server to use the Bootstrap Token for authentication for certain sensitive operations; for example, enabling kernel extensions or installing certain types of software updates. Set this value to `false` if your MDM server doesn’t need to perform these operations. The value provided here overrides the value specified in MDM, and only applies when `BootstrapTokenAllowedForAuthentication` is `true` in the SecurityInfoResponse.SecurityInfo response. This value is available for Apple silicon in macOS 11 and later.

Default: `false`

## Discussion

This command sets the dictionary as the complete set of options. It doesn’t merge keys between multiple MDM options commands.

