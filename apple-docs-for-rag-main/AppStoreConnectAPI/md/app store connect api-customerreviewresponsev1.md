

- App Store Connect API
-  CustomerReviewResponseV1 

Object

# CustomerReviewResponseV1

The data structure that represents the Customer Review Responses resource.

App Store Connect API 2.0+

``` source
object CustomerReviewResponseV1
```

## Properties

`attributes`

CustomerReviewResponseV1.Attributes

The attributes of the response to the customer’s review, including its content.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the `CustomerReviewResponses` resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

CustomerReviewResponseV1.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `customerReviewResponses`

## Topics

### Objects

object CustomerReviewResponseV1.Attributes

The attributes of the response to a customer’s review including its content.

object CustomerReviewResponseV1.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Types

object CustomerReviewResponseV1Response

A response that contains a single Customer Review Responses resource.

object CustomerReviewResponseV1CreateRequest

The request body to use to create a response to a customer review.

object CustomerReview

The data structure that represents a Customer Reviews resource.

