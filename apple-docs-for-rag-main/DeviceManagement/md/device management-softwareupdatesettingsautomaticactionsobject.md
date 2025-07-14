

- Device Management
-  SoftwareUpdateSettingsAutomaticActionsObject 

Object

# SoftwareUpdateSettingsAutomaticActionsObject

The object that configures various automatic Software Update functionality.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdateSettingsAutomaticActionsObject
```

## Properties

`Download`

`string`

Specifies whether the user can control automatic downloads of available updates:

- `Allowed` - the user can enable or disable automatic downloads.

- `AlwaysOn` - automatic downloads are always enabled.

- `AlwaysOff` - automatic downloads are always disabled.

Default: `Allowed`

Possible Values: `Allowed, AlwaysOn, AlwaysOff`

`InstallOSUpdates`

`string`

Specifies whether the user can control automatic installation of available updates:

- `Allowed` - the user can enable or disable automatic installation.

- `AlwaysOn` - automatic installations are always enabled.

- `AlwaysOff` - automatic installations are always disabled.

Default: `Allowed`

Possible Values: `Allowed, AlwaysOn, AlwaysOff`

`InstallSecurityUpdate`

`string`

Specifies whether the user can control automatic installation of available security updates:

- `Allowed` - the user can enable or disable automatic installation.

- `AlwaysOn` - automatic installations are always enabled.

- `AlwaysOff` - automatic installations are always disabled.

Default: `Allowed`

Possible Values: `Allowed, AlwaysOn, AlwaysOff`

## See Also

### Supporting Objects

object SoftwareUpdateSettingsBetaObject

The object that configures overall beta program settings.

object SoftwareUpdateSettingsBeta_ProgramObject

The object that configures a specific beta program.

object SoftwareUpdateSettingsBeta_RequireProgramObject

The object that configures beta program requirement settings.

object SoftwareUpdateSettingsDeferralsObject

The object that configures update deferrals.

object SoftwareUpdateSettingsRapidSecurityResponseObject

The object that configures rapid security update settings.

