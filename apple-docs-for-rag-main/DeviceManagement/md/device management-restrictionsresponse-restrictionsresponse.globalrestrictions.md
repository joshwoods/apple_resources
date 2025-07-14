

- Device Management
- RestrictionsResponse
-  RestrictionsResponse.GlobalRestrictions 

Device Management Command

# RestrictionsResponse.GlobalRestrictions

A dictionary that contains the global restrictions in effect.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RestrictionsResponse.GlobalRestrictions
```

## Properties

`intersection`

RestrictionsResponse.GlobalRestrictions.Intersection

A dictionary of intersected restrictions. Intersected restrictions indicate that new restrictions can only reduce the number of strings in the set.

`restrictedBool`

RestrictionsResponse.GlobalRestrictions.RestrictedBool

A dictionary of Boolean restrictions.

`restrictedValue`

RestrictionsResponse.GlobalRestrictions.RestrictedValue

A dictionary of numeric restrictions.

`union`

RestrictionsResponse.GlobalRestrictions.Union

A dictionary of unioned restrictions. Unioned restrictions indicate that new restrictions can add to the set.

## Topics

### Commands

object RestrictionsResponse.GlobalRestrictions.Intersection

A dictionary that contains intersected restrictions.

object RestrictionsResponse.GlobalRestrictions.RestrictedBool

A dictionary that contains Boolean restrictions.

object RestrictionsResponse.GlobalRestrictions.RestrictedValue

A dictionary that contains numeric restrictions.

object RestrictionsResponse.GlobalRestrictions.Union

A dictionary that contains unioned restrictions.

## See Also

### Commands

object RestrictionsResponse.ProfileRestrictions

A dictionary that contains restrictions from each profile.

object RestrictionsResponse.ErrorChainItem

A dictionary that describes an error chain.

