

- Apple News API
-  Throttling 

Object

# Throttling

See the object that wraps the throttling information that’s returned for the Create an Article and Update an Article endpoints.

Apple News API 1.0+

``` source
object Throttling
```

## Properties

`estimatedDelayInSeconds`

`integer`

Estimate of the number of seconds until this request begins processing.

`isThrottled`

`boolean`

A Boolean value that indicates whether requests to this channel are currently being throttled. If `true`, the server adds this request to the queue to process later rather than immediately.

Default: `false`

`queueSize`

`integer`

The number of requests currently queued for later processing.

Minimum: `0`

`quotaAvailable`

`integer`

The number of additional article publish or update requests that you can submit now, before the system begins throttling.

## See Also

### Articles

Create an Article

Publish an article to your channel.

Read Article Information

Retrieve information about an article, such as the revision number and maturity rating.

Search Articles in a Channel

See a list of all articles in a channel that match the specified search criteria.

Search Articles in a Section

See a list of all articles in a section that match the specified search criteria.

Update an Article

Update an existing article in your channel.

Delete an Article

Delete the specified article from your channel.

object Create Article Metadata Fields

See the optional metadata fields for the Create an Article Request.

object ArticleLinksRequest

See the required field for the Create an Article request.

object Update Article Metadata Fields

See the metadata fields for the Update an Article request.

object Article

See the fields the article endpoints returned.

object ArticleResponse

See which objects make up the Create an Article, Read an Article, and Update an Article responses.

object ArticleLinksResponse

See the links the article endpoints returned.

object SearchResponse

See the fields the search article endpoints returned.

object Meta

See the object that wraps the throttling information that’s returned for the Create an Article and Read an Article endpoints.

