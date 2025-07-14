

- App Store Connect API
- CustomerReviewResponseV1CreateRequest
- 
  - CustomerReviewResponseV1CreateRequest
- CustomerReviewResponseV1CreateRequest.Data
- CustomerReviewResponseV1CreateRequest.Data.Relationships
- CustomerReviewResponseV1CreateRequest.Data.Relationships.Review
-  CustomerReviewResponseV1CreateRequest.Data.Relationships.Review.Data 

Object

# CustomerReviewResponseV1CreateRequest.Data.Relationships.Review.Data

The type and ID of a resource that you’re relating with the resource you’re updating.

App Store Connect API 2.0+

``` source
object CustomerReviewResponseV1CreateRequest.Data.Relationships.Review.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the `customerReviews` resource that you’re responding to.

`type`

`string`

 (Required) 

The resource type.

Value: `customerReviews`

