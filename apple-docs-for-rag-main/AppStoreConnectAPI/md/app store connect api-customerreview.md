

- App Store Connect API
-  CustomerReview 

Object

# CustomerReview

The data structure that represents a Customer Reviews resource.

App Store Connect API 2.0+

``` source
object CustomerReview
```

## Properties

`attributes`

CustomerReview.Attributes

The attributes of the customer’s review including its content.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the `CustomerReviews` resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

CustomerReview.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `customerReviews`

## Topics

### Objects

object CustomerReview.Attributes

The attributes of the customer’s review including its content.

object CustomerReview.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Types

object CustomerReviewResponseV1Response

A response that contains a single Customer Review Responses resource.

object CustomerReviewResponseV1

The data structure that represents the Customer Review Responses resource.

object CustomerReviewResponseV1CreateRequest

The request body to use to create a response to a customer review.

