

- Apple News API
-  Delete an Article 

Web Service Endpoint

# Delete an Article

Delete the specified article from your channel.

Apple News API 1.0+

## URL

``` source
DELETE https://news-api.apple.com/articles/{articleId}
```

## Path Parameters

`articleId`

`string`

 (Required) 

The UUID or the Share URL ID of the article you want to delete. The server returns the article ID and the Share URL when you create an article (see Create an Article) and in Read Article Information and Update an Article responses.

## Response Codes

` 204 ``No Content`

`No Content`

The request was successful but there was no response in the body.

` 400 ``Bad Request`

Error

`Bad Request`

- You didn’t include the article `UUID` or the Share URL ID field in the request. Key path: \*

- The Apple News team optimized the article, so your article wasn’t deleted. Contact your Apple News technical representative if you need to delete it.

Content-Type: application/json

` 401 ``Unauthorized`

Error

`Unauthorized`

You didn’t include the `Authorization` header. Key path: N/A

Content-Type: application/json

` 403 ``Forbidden`

Error

`Forbidden`

You tried to access an article your API key doesn’t have permission to access. Key path: N/A

Content-Type: application/json

` 404 ``Not Found`

Error

`Not Found`

- The endpoint you tried to access doesn’t exist. Key path: N/A

- The article you tried to access doesn’t exist. Key path: `articleId`.

Content-Type: application/json

## Mentioned in 

Apple News API Release Notes for iOS 17, iPadOS 17, and macOS 14

## Discussion

If the article is viewed on a device, it may take some time for the News app to refresh the cache so the article disappears on that device.

Important

Once you delete the specified article, the action is irrevocable. If you want to remove the article temporarily, use the update operation with `isHidden` set to `true`. See Update an Article and Update Article Metadata Fields.

### Example

- Request
- Response

```
DELETE /articles/a3caeb08-b9db-4002-b379-cde305d74be7 HTTP/1.1
Host: news-api.apple.com
Accept: application/json
Authorization: HHMAC; key="1e3gfc5e-e9f8-4232-a6be-17bf40edad09"; signature="irqw07DCRQLtx/40Z2VhNc7sl3nB1PKII374R7AHjUQ="; date="2015-02-28T00:03:31Z"
```

```
HTTP/1.1 204 No Content
Date: Sat, 28 Feb 2015 00:51:41 GMT
```

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

object Throttling

See the object that wraps the throttling information that’s returned for the Create an Article and Update an Article endpoints.

