

- App Store Connect API
-  CustomerReviewsResponse 

Object

# CustomerReviewsResponse

A response that contains a list of Customer Reviews resources.

App Store Connect API 2.0+

``` source
object CustomerReviewsResponse
```

## Properties

`data`

`[`CustomerReview`]`

 (Required) 

A list of customer review resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[`CustomerReviewResponseV1`]`

The requested relationship data.

## See Also

### Objects

object CustomerReviewResponse

A response that contains a single Customer Review resource.

object CustomerReview

The data structure that represents a Customer Reviews resource.

