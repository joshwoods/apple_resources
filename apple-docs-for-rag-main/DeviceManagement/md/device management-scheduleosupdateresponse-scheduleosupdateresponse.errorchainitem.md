

- Device Management
- ScheduleOSUpdateResponse
-  ScheduleOSUpdateResponse.ErrorChainItem 

Device Management Command

# ScheduleOSUpdateResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object ScheduleOSUpdateResponse.ErrorChainItem
```

## Properties

`ErrorCode`

`integer`

 (Required) 

The error code.

`ErrorDomain`

`string`

 (Required) 

The error domain.

`LocalizedDescription`

`string`

 (Required) 

A description of the error in the device’s localized language.

`USEnglishDescription`

`string`

A description of the error in U.S. English.

## See Also

### Commands

object ScheduleOSUpdateResponse.UpdateResultsItem

The response dictionary that describes the result of processing an operating-system update.

