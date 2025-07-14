

- Device Management
- ManagedApplicationConfigurationResponse
-  ManagedApplicationConfigurationResponse.ErrorChainItem 

Device Management Command

# ManagedApplicationConfigurationResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 7.0+iPadOS 7.0+macOS 10.15+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationConfigurationResponse.ErrorChainItem
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

object ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem

A dictionary that contains a managed app’s configurations item.

