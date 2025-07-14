

- App Store Connect API
-  AppsBetaTesterUsagesV1MetricResponse 

Object

# AppsBetaTesterUsagesV1MetricResponse

A response that contains one or more beta app tester metric resources.

App Store Connect API 3.1+

``` source
object AppsBetaTesterUsagesV1MetricResponse
```

## Properties

`data`

`[`AppsBetaTesterUsagesV1MetricResponse.Data`]`

 (Required) 

`included`

`[`BetaTester`]`

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## Topics

### Objects

object AppsBetaTesterUsagesV1MetricResponse.Data

## See Also

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

object BetaTestersResponse

A response that contains a list of Beta Tester resources.

object BetaTesterUsagesV1MetricResponse

A response that contains one or more beta tester usage metric resources.

