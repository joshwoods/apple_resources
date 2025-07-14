

- Device Management
- ManagedApplicationAttributesResponse
-  ManagedApplicationAttributesResponse.ErrorChainItem 

Device Management Command

# ManagedApplicationAttributesResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 7.0+iPadOS 7.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationAttributesResponse.ErrorChainItem
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

object ManagedApplicationAttributesResponse.ApplicationAttributesItem

A dictionary that contains a managed app attributes item.

