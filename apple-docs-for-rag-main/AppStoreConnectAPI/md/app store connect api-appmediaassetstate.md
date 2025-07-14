

- App Store Connect API
-  AppMediaAssetState 

Object

# AppMediaAssetState

The state of an app or media upload, including any errors and warnings.

App Store Connect API 1.2+

``` source
object AppMediaAssetState
```

## Properties

`errors`

`[`AppMediaStateError`]`

`state`

`string`

Possible Values: `AWAITING_UPLOAD, UPLOAD_COMPLETE, COMPLETE, FAILED`

`warnings`

`[`AppMediaStateError`]`

## See Also

### Objects

object RoutingAppCoverage

The data structure that represents the Routing App Coverages resource.

object RoutingAppCoverageWithoutIncludesResponse

object RoutingAppCoverageCreateRequest

The request body you use to create a Routing App Coverage.

object RoutingAppCoverageResponse

A response that contains a single Routing App Coverages resource.

object RoutingAppCoverageUpdateRequest

The request body you use to update a Routing App Coverage.

object AppMediaStateError

An error code and description.

