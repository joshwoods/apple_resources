

- Apple News API
-  ArticleLinksResponse 

Object

# ArticleLinksResponse

See the links the article endpoints returned.

Apple News API 2.2+

``` source
object ArticleLinksResponse
```

## Properties

`channel`

`string`

The URL of the channel in which this article appears.

`sections`

`[string]`

The URL of the sections, if any, in which this article appears.

`self`

`string`

The URL at which you can read, update, or delete the article.

## Relationships

### Inherited By

- ArticleResponse

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

object SearchResponse

See the fields the search article endpoints returned.

object Meta

See the object that wraps the throttling information that’s returned for the Create an Article and Read an Article endpoints.

object Throttling

See the object that wraps the throttling information that’s returned for the Create an Article and Update an Article endpoints.

