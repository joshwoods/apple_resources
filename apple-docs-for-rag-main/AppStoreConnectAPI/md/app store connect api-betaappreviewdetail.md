

- App Store Connect API
-  BetaAppReviewDetail 

Object

# BetaAppReviewDetail

The data structure that represents a Beta App Review Details resource.

App Store Connect API 1.0+

``` source
object BetaAppReviewDetail
```

## Properties

`attributes`

BetaAppReviewDetail.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

BetaAppReviewDetail.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaAppReviewDetails`

## Topics

### Objects

object BetaAppReviewDetail.Attributes

Attributes that describe a Beta App Review Details resource.

object BetaAppReviewDetail.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BetaAppReviewDetailUpdateRequest

The request body you use to update a Beta App Review Detail.

object BetaAppReviewDetailResponse

A response that contains a single Beta App Review Details resource.

object BetaAppReviewDetailWithoutIncludesResponse

object BetaAppReviewDetailsResponse

A response that contains a list of Beta App Review Detail resources.

object AppBetaTestersLinkagesRequest

A request body you use to remove beta testers from an app.

