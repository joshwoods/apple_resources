

- App Store Connect API
-  BetaGroupResponse 

Object

# BetaGroupResponse

A response that contains a single Beta Groups resource.

App Store Connect API 1.0+

``` source
object BetaGroupResponse
```

## Properties

`data`

BetaGroup

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[*]`

Possible types: App`, `Build`, `BetaTester`, `BetaRecruitmentCriterion

## See Also

### Related Documentation

Create a Beta Group

Create a beta group associated with an app, optionally enabling TestFlight public links.

### Objects

object BetaGroup

The data structure that represents a Beta Groups resource.

object BetaGroupsWithoutIncludesResponse

A response body that contains a list of beta groups without any includes.

object BetaGroupCreateRequest

The request body you use to create a Beta Group.

object BetaGroupUpdateRequest

The request body you use to update a Beta Group.

object BetaGroupBuildsLinkagesRequest

A request body you use to add or remove builds from a beta group.

object BetaGroupBetaTestersLinkagesRequest

A request body you use to add or remove beta testers from a beta group.

object BetaGroupBetaTestersLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaGroupBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaPublicLinkUsagesV1MetricResponse

object BetaGroupsResponse

A response that contains a list of Beta Group resources.

