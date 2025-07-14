

- App Store Connect API
-  CiBuildActionResponse 

Object

# CiBuildActionResponse

A response that contains a single Build Actions resource.

App Store Connect API 1.5+

``` source
object CiBuildActionResponse
```

## Properties

`data`

CiBuildAction

 (Required) 

The resource data.

`included`

`[`CiBuildRun`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object CiBuildAction

The data structure that represents a Build Actions resource.

object CiArtifactsResponse

A response that contains a list of Artifacts resources.

object CiIssuesResponse

A response that contains a list of Issues resources.

object CiTestResultsResponse

A response that contains a list of Test Results resources.

