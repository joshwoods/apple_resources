

- App Store Connect API
- BetaGroupCreateRequest
- BetaGroupCreateRequest.Data
-  BetaGroupCreateRequest.Data.Attributes 

Object

# BetaGroupCreateRequest.Data.Attributes

Attributes that you set that describe the new beta group resource.

App Store Connect API 1.0+

``` source
object BetaGroupCreateRequest.Data.Attributes
```

## Properties

`name`

`string`

 (Required) 

The name for the beta group.

`publicLinkEnabled`

`boolean`

Only applicable to external groups. A Boolean value that indicates whether a public link is enabled. Enable a link to invite anyone outside of your team to beta test your app. When you share this link, testers can install the beta version of your app on their devices in TestFlight and share the link with others.

`publicLinkLimit`

`integer`

Only applicable to external groups. The maximum number of testers that can join this beta group using the public link. Values must be between 1 and 10,000.

`publicLinkLimitEnabled`

`boolean`

Only applicable to external groups. A Boolean value that limits the number of testers who can join the beta group using the public link.

`feedbackEnabled`

`boolean`

`hasAccessToAllBuilds`

`boolean`

`isInternalGroup`

`boolean`

## See Also

### Objects

object BetaGroupCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

