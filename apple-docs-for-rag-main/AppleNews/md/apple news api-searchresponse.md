

- Apple News API
-  SearchResponse 

Object

# SearchResponse

See the fields the search article endpoints returned.

Apple News API 1.0+

``` source
object SearchResponse
```

## Properties

`articles`

`[`Article`]`

A list of article objects.

`links`

SearchResponse.Links

A list of fields the Search Articles in a Section and Search Articles in a Channel endpoints return.

`meta`

`string`

The value you want to set for the `pageToken` parameter and the parameters that were previously sent to get the next page of results. This field is automatically filled in with the next URL in the links section.

## Topics

### Objects

object SearchResponse.Links

See the links the search article endpoints returned.

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

object Meta

See the object that wraps the throttling information that’s returned for the Create an Article and Read an Article endpoints.

object Throttling

See the object that wraps the throttling information that’s returned for the Create an Article and Update an Article endpoints.

