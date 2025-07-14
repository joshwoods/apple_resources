

- App Store Connect API
-  BetaTestersResponse 

Object

# BetaTestersResponse

A response that contains a list of Beta Tester resources.

App Store Connect API 1.0+

``` source
object BetaTestersResponse
```

## Properties

`data`

`[`BetaTester`]`

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

Possible types: App`, `BetaGroup`, `Build

## See Also

### Related Documentation

List All Beta Testers in a Beta Group

Get a list of beta testers contained in a specific beta group.

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

object BetaTesterBetaGroupsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterBuildsLinkagesRequest

A request body you use to add or remove builds from a beta tester.

object BetaTesterBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterCreateRequest

The request body you use to create a BetaTester.

object BetaTesterResponse

A response that contains a single Beta Testers resource.

object AppsBetaTesterUsagesV1MetricResponse

A response that contains one or more beta app tester metric resources.

object BetaTesterUsagesV1MetricResponse

A response that contains one or more beta tester usage metric resources.

