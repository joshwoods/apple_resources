

- App Store Connect API
- CustomerReviewResponseV1CreateRequest
-  CustomerReviewResponseV1CreateRequest.Data 

Object

# CustomerReviewResponseV1CreateRequest.Data

The data element of the request body for creating a response to a customer review.

App Store Connect API 2.0+

``` source
object CustomerReviewResponseV1CreateRequest.Data
```

## Properties

`attributes`

CustomerReviewResponseV1CreateRequest.Data.Attributes

 (Required) 

The attributes of the customer review response, including its text content.

`relationships`

CustomerReviewResponseV1CreateRequest.Data.Relationships

 (Required) 

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `customerReviewResponses`

## Topics

### Objects

object CustomerReviewResponseV1CreateRequest.Data.Attributes

The attributes of the customer review response, including its text content.

object CustomerReviewResponseV1CreateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

