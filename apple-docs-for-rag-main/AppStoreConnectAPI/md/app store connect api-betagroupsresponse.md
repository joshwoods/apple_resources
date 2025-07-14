

- App Store Connect API
-  BetaGroupsResponse 

Object

# BetaGroupsResponse

A response that contains a list of Beta Group resources.

App Store Connect API 1.0+

``` source
object BetaGroupsResponse
```

## Properties

`data`

`[`BetaGroup`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[*]`

Possible types: App`, `Build`, `BetaTester`, `BetaRecruitmentCriterion

## See Also

### Related Documentation

List Beta Groups

Find and list beta groups for all apps.

### Objects

object BetaGroup

The data structure that represents a Beta Groups resource.

object BetaGroupResponse

A response that contains a single Beta Groups resource.

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

