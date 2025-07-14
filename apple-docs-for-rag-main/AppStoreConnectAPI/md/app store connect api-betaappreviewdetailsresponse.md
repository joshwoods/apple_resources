

- App Store Connect API
-  BetaAppReviewDetailsResponse 

Object

# BetaAppReviewDetailsResponse

A response that contains a list of Beta App Review Detail resources.

App Store Connect API 1.0+

``` source
object BetaAppReviewDetailsResponse
```

## Properties

`data`

`[`BetaAppReviewDetail`]`

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

`[`App`]`

## See Also

### Related Documentation

List Beta App Review Details

Find and list beta app review details for all apps.

### Objects

object BetaAppReviewDetail

The data structure that represents a Beta App Review Details resource.

object BetaAppReviewDetailUpdateRequest

The request body you use to update a Beta App Review Detail.

object BetaAppReviewDetailResponse

A response that contains a single Beta App Review Details resource.

object BetaAppReviewDetailWithoutIncludesResponse

object AppBetaTestersLinkagesRequest

A request body you use to remove beta testers from an app.

