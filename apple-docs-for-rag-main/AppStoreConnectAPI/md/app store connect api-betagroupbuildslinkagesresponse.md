

- App Store Connect API
-  BetaGroupBuildsLinkagesResponse 

Object

# BetaGroupBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

App Store Connect API 1.0+

``` source
object BetaGroupBuildsLinkagesResponse
```

## Properties

`data`

`[`BetaGroupBuildsLinkagesResponse.Data`]`

 (Required) 

The object types and IDs of the related resources.

`links`

PagedDocumentLinks

 (Required) 

Navigational links including the self-link and links to the related data.

`meta`

PagingInformation

Paging information.

## Topics

### Objects

object BetaGroupBuildsLinkagesResponse.Data

The data element of the response body.

## See Also

### Related Documentation

Get All Build IDs in a Beta Group

Get a list of build resource IDs in a specific beta group.

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

object BetaPublicLinkUsagesV1MetricResponse

object BetaGroupsResponse

A response that contains a list of Beta Group resources.

