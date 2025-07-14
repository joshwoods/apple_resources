

- App Store Connect API
-  BetaGroupsWithoutIncludesResponse 

Object

# BetaGroupsWithoutIncludesResponse

A response body that contains a list of beta groups without any includes.

App Store Connect API 3.0+

``` source
object BetaGroupsWithoutIncludesResponse
```

## Properties

`data`

`[`BetaGroup`]`

 (Required) 

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object BetaGroup

The data structure that represents a Beta Groups resource.

object BetaGroupResponse

A response that contains a single Beta Groups resource.

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

