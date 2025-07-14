

- Device Management
-  SoftwareUpdateSettingsRapidSecurityResponseObject 

Object

# SoftwareUpdateSettingsRapidSecurityResponseObject

The object that configures rapid security update settings.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdateSettingsRapidSecurityResponseObject
```

## Properties

`Enable`

`boolean`

If set to `false`, Rapid Security Responses aren’t offered for user installation. The system can still install Rapid Security Responses with `com.apple.configuration.softwareupdate.enforcement.specific` configurations.

If set to `true`, the system offers Rapid Security Responses to the user.

Default: `true`

`EnableRollback`

`boolean`

If set to `false`, the system doesn’t offer Rapid Security Response rollbacks to the user.

If set to `true`, the system offers Rapid Security Response rollbacks to the user.

Default: `true`

## See Also

### Supporting Objects

object SoftwareUpdateSettingsAutomaticActionsObject

The object that configures various automatic Software Update functionality.

object SoftwareUpdateSettingsBetaObject

The object that configures overall beta program settings.

object SoftwareUpdateSettingsBeta_ProgramObject

The object that configures a specific beta program.

object SoftwareUpdateSettingsBeta_RequireProgramObject

The object that configures beta program requirement settings.

object SoftwareUpdateSettingsDeferralsObject

The object that configures update deferrals.

