

- App Store Connect API
-  CustomerReviewResponse 

Object

# CustomerReviewResponse

A response that contains a single Customer Review resource.

App Store Connect API 2.0+

``` source
object CustomerReviewResponse
```

## Properties

`data`

CustomerReview

 (Required) 

The data structure that represents a `CustomerReviews` resource.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[`CustomerReviewResponseV1`]`

The requested relationship data.

## See Also

### Objects

object CustomerReviewsResponse

A response that contains a list of Customer Reviews resources.

object CustomerReview

The data structure that represents a Customer Reviews resource.

