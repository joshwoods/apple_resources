

- App Store Connect API
-  BetaTesterBetaGroupsLinkagesResponse 

Object

# BetaTesterBetaGroupsLinkagesResponse

A response body that contains a list of related resource IDs.

App Store Connect API 1.0+

``` source
object BetaTesterBetaGroupsLinkagesResponse
```

## Properties

`data`

`[`BetaTesterBetaGroupsLinkagesResponse.Data`]`

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

object BetaTesterBetaGroupsLinkagesResponse.Data

The data element of the response body.

## See Also

### Related Documentation

Get All Beta Group IDs of a Beta Tester's Groups

Get a list of group resource IDs associated with a beta tester.

### Objects

object BetaTester

The data structure that represents a Beta Testers resource.

object BetaTestersWithoutIncludesResponse

object BetaTesterAppsLinkagesRequest

A request body you use to remove an app from a beta tester.

object BetaTesterAppsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterBetaGroupsLinkagesRequest

A request body you use to add or remove beta groups from a beta tester.

object BetaTesterBuildsLinkagesRequest

A request body you use to add or remove builds from a beta tester.

object BetaTesterBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterCreateRequest

The request body you use to create a BetaTester.

object BetaTesterResponse

A response that contains a single Beta Testers resource.

object BetaTestersResponse

A response that contains a list of Beta Tester resources.

object AppsBetaTesterUsagesV1MetricResponse

A response that contains one or more beta app tester metric resources.

object BetaTesterUsagesV1MetricResponse

A response that contains one or more beta tester usage metric resources.

