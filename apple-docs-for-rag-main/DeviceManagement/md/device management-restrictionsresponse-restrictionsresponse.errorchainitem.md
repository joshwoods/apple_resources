

- Device Management
- RestrictionsResponse
-  RestrictionsResponse.ErrorChainItem 

Device Management Command

# RestrictionsResponse.ErrorChainItem

A dictionary that describes an error chain.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RestrictionsResponse.ErrorChainItem
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

object RestrictionsResponse.GlobalRestrictions

A dictionary that contains the global restrictions in effect.

object RestrictionsResponse.ProfileRestrictions

A dictionary that contains restrictions from each profile.

