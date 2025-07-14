

- Device Management
- RestrictionsResponse
- RestrictionsResponse.ProfileRestrictions
-  RestrictionsResponse.ProfileRestrictions.ANY profile identifier 

Device Management Command

# RestrictionsResponse.ProfileRestrictions.ANY profile identifier

A dictionary that contains profile restrictions in effect.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RestrictionsResponse.ProfileRestrictions.ANY profile identifier
```

## Properties

`intersection`

RestrictionsResponse.ProfileRestrictions.ANY profile identifier.Intersection

A dictionary of intersected profile restrictions. Intersected restrictions indicate that new restrictions can only reduce the number of strings in the set.

`restrictedBool`

RestrictionsResponse.ProfileRestrictions.ANY profile identifier.RestrictedBool

A dictionary of Boolean profile restrictions.

`restrictedValue`

RestrictionsResponse.ProfileRestrictions.ANY profile identifier.RestrictedValue

A dictionary of numeric profile restrictions.

`union`

RestrictionsResponse.ProfileRestrictions.ANY profile identifier.Union

A dictionary of unioned profile restrictions. Unioned restrictions indicate that new restrictions can add to the set.

## Topics

### Commands

object RestrictionsResponse.ProfileRestrictions.ANY profile identifier.Intersection

A dictionary that contains intersected profile restrictions.

object RestrictionsResponse.ProfileRestrictions.ANY profile identifier.RestrictedBool

A dictionary that contains Boolean profile restrictions.

object RestrictionsResponse.ProfileRestrictions.ANY profile identifier.RestrictedValue

A dictionary that contains numeric profile restrictions.

object RestrictionsResponse.ProfileRestrictions.ANY profile identifier.Union

A dictionary that contains unioned profile restrictions.

