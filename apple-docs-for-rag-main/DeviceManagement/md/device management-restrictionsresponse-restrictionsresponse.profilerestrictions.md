

- Device Management
- RestrictionsResponse
-  RestrictionsResponse.ProfileRestrictions 

Device Management Command

# RestrictionsResponse.ProfileRestrictions

A dictionary that contains restrictions from each profile.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RestrictionsResponse.ProfileRestrictions
```

## Properties

`ANY profile identifier`

RestrictionsResponse.ProfileRestrictions.ANY profile identifier

The profile identifiers.

## Discussion

This dictionary is only available if `ProfileRestrictions` is `true` in the command.

## Topics

### Commands

object RestrictionsResponse.ProfileRestrictions.ANY profile identifier

A dictionary that contains profile restrictions in effect.

## See Also

### Commands

object RestrictionsResponse.GlobalRestrictions

A dictionary that contains the global restrictions in effect.

object RestrictionsResponse.ErrorChainItem

A dictionary that describes an error chain.

