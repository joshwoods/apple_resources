

- Device Management
-  SoftwareUpdateSettingsBeta_RequireProgramObject 

Object

# SoftwareUpdateSettingsBeta_RequireProgramObject

The object that configures beta program requirement settings.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdateSettingsBeta_RequireProgramObject
```

## Properties

`Description`

`string`

 (Required) 

A human readable description of the beta program.

`Token`

`string`

 (Required) 

The Apple Business Manager or Apple School Manager seeding service token for the organization the MDM server is part of. The system uses this token to enroll the device in the corresponding beta program.

## See Also

### Supporting Objects

object SoftwareUpdateSettingsAutomaticActionsObject

The object that configures various automatic Software Update functionality.

object SoftwareUpdateSettingsBetaObject

The object that configures overall beta program settings.

object SoftwareUpdateSettingsBeta_ProgramObject

The object that configures a specific beta program.

object SoftwareUpdateSettingsDeferralsObject

The object that configures update deferrals.

object SoftwareUpdateSettingsRapidSecurityResponseObject

The object that configures rapid security update settings.

