

- App Store Connect API
- BetaGroup
-  BetaGroup.Attributes 

Object

# BetaGroup.Attributes

Attributes with values that describe a beta group update request.

App Store Connect API 1.0+

``` source
object BetaGroup.Attributes
```

## Properties

`isInternalGroup`

`boolean`

A Boolean value that indicates whether the group is internal. Only existing users of App Store Connect may be added for internal beta testing.

`name`

`string`

The name for the beta group.

`publicLink`

`string`

The URL of the public link provided to your app’s beta testers.

`publicLinkEnabled`

`boolean`

A Boolean value that indicates whether a public link is enabled. Enable a link to invite anyone outside of your team to beta test your app. When you share this link, testers can install the beta version of your app on their devices in TestFlight and share the link with others.

`publicLinkId`

`string`

The ID as part of the URL of the public link.

`publicLinkLimit`

`integer`

The maximum number of testers that can join this beta group using the public link. Values must be between 1 and 10,000.

`publicLinkLimitEnabled`

`boolean`

A Boolean value that limits the number of testers who can join the beta group using the public link.

`createdDate`

`date-time`

The creation date of the beta group.

`feedbackEnabled`

`boolean`

`hasAccessToAllBuilds`

`boolean`

`iosBuildsAvailableForAppleSiliconMac`

`boolean`

`iosBuildsAvailableForAppleVision`

`boolean`

## Mentioned in 

App Store Connect API 1.5 release notes

## See Also

### Related Documentation

Beta Groups

Groups of beta testers that have access to one or more builds.

### Objects

object BetaGroup.Relationships

The relationships you included in the request and those on which you can operate.

