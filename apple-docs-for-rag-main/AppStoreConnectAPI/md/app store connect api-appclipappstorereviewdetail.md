

- App Store Connect API
-  AppClipAppStoreReviewDetail 

Object

# AppClipAppStoreReviewDetail

The data structure that represents an App Clip App Store Review Details resource.

App Store Connect API 1.6+

``` source
object AppClipAppStoreReviewDetail
```

## Properties

`attributes`

AppClipAppStoreReviewDetail.Attributes

The attributes that describe the App Clip App Store Review Details resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an App Clip App Store Review Details resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppClipAppStoreReviewDetail.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipAppStoreReviewDetails`

## Topics

### Objects

object AppClipAppStoreReviewDetail.Attributes

The attributes that describe the App Clip App Store Review Details resource.

object AppClipAppStoreReviewDetail.Relationships

The relationships of the App Clip App Store Details resource you included in the request and those on which you can operate.

## See Also

### Objects

object AppClipAppStoreReviewDetailResponse

A response that contains a single App Clip App Store Review Details resource.

object AppClipAppStoreReviewDetailCreateRequest

The request body you use to create an App Clip App Store Review Detail.

object AppClipAppStoreReviewDetailUpdateRequest

The request body you use to update App Clip information that you provide to App Store Review.

