

- App Store Connect API
-  CustomerReviewResponseV1Response 

Object

# CustomerReviewResponseV1Response

A response that contains a single Customer Review Responses resource.

App Store Connect API 2.0+

``` source
object CustomerReviewResponseV1Response
```

## Properties

`data`

CustomerReviewResponseV1

 (Required) 

The data structure that represents a `CustomerReviewResponses` resource.

`included`

`[`CustomerReview`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects and Types

object CustomerReviewResponseV1

The data structure that represents the Customer Review Responses resource.

object CustomerReviewResponseV1CreateRequest

The request body to use to create a response to a customer review.

object CustomerReview

The data structure that represents a Customer Reviews resource.

