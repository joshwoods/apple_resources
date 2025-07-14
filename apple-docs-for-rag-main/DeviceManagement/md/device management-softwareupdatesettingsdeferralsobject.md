

- Device Management
-  SoftwareUpdateSettingsDeferralsObject 

Object

# SoftwareUpdateSettingsDeferralsObject

The object that configures update deferrals.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdateSettingsDeferralsObject
```

## Properties

`CombinedPeriodInDays`

`integer`

Specifies the number of days to defer a major or minor OS software update on the device. When set, software updates only appear after the specified delay, following the release of the software update. Available in iOS 18 and later.

Minimum: `1`

Maximum: `90`

`MajorPeriodInDays`

`integer`

Specifies the number of days to defer a major OS software update on the device. When set, software updates only appear after the specified delay, following the release of the software update. Available in macOS 15 and later.

Minimum: `1`

Maximum: `90`

`MinorPeriodInDays`

`integer`

Specifies the number of days to defer a minor OS software update on the device. It also defers major updates for iOS. When set, software updates only appear after the specified delay, following the release of the software update. Available in macOS 15 and later.

Minimum: `1`

Maximum: `90`

`SystemPeriodInDays`

`integer`

Specifies the number of days to defer system or non-OS updates. When set, updates only appear after the specified delay, following the release of the update. Available in macOS 15 and later.

Minimum: `1`

Maximum: `90`

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

object SoftwareUpdateSettingsRapidSecurityResponseObject

The object that configures rapid security update settings.

