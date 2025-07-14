

- Apple News API
-  Promote Articles in a Section 

Web Service Endpoint

# Promote Articles in a Section

Set the list of promoted articles for the specified section.

Apple News API 1.0+

## URL

``` source
POST https://news-api.apple.com/sections/{sectionId}/promotedArticles
```

## Path Parameters

`sectionId`

`string`

 (Required) 

The UUID of the section.

## HTTP Body

PromoteArticleRequest

The list of IDs for articles you want to promote.

Content-Type: application/json

## Response Codes

` 200 ``OK`

PromoteArticleResponse

`OK`

The request was successful.

Content-Type: application/json

` 400 ``Bad Request`

Error

`Bad Request`

The specified article ID isn’t a valid `UUID`.

Key path: `data.promotedArticle.`

Content-Type: application/json

` 401 ``Unauthorized`

Error

`Unauthorized`

You didn’t include the `Authorization` header.

Key path: None.

Content-Type: application/json

` 403 ``Forbidden`

Error

`Forbidden`

The channel doesn’t have permission to promote the article.

Key path: `data.promotedArticle.`

Value: `Invalid ID.`

Content-Type: application/json

` 404 ``Not Found`

Error

`Not Found`

- The endpoint you tried to access doesn’t exist. Key path: None.

- `NOT_FOUND`. The specified section ID doesn’t exist. Key path: None. Value: None.

- `NOT_FOUND`. The article with the specified ID doesn’t exist. Key path: `data.promotedArticle.` Value: `Article ID.`

Content-Type: application/json

` 422 `

Error

`MISSING_THUMBNAIL_FOR_PROMOTED_ARTICLE`. The list of articles you promoted has at least one article without a thumbnail image.

Key path: `data.promotedArticles.`

Content-Type: application/json

## Discussion

A Promote Articles in a Section request sets the list of promoted articles for the specified section. You can promote up to six articles per section. Note that each article promoted in a section should have a thumbnail image. The system generates an error if an article in the list doesn’t include a thumbnail image. The list of articles given in the body of this request replaces any previous list of promoted articles. You can remove the list of promoted articles for the section by specifying an empty list. The promoted articles list is valid for a system-defined time period after it is set.

The request body must be in JSON, in the following format:

```
{
  "data": {
    "promotedArticles": [
      "F59D1784-CAFC-432A-9A1A-EF2FCE1E1C60",
      "2027DD1B-2794-4B0A-B9DC-F7EE696411FF"
    ]
  }
}
```

### Example

- Request
- Response

```
POST /sections/a3caeb08-b9db-4002-b379-cde305d74be7/promotedArticles HTTP/1.1
Host: news-api.apple.com
Accept: application/json
Authorization: HHMAC; key="1e3gfc5e-e9f8-4232-a6be-17bf40edad09";
signature="irqw07DCRQLtx/40Z2VhNc7sl3nB1PKII374R7AHjUQ=";
date="2017-12-08T00:03:31Z"
{
  "data": {
    "promotedArticles": [
      "F59D1784-CAFC-432A-9A1A-EF2FCE1E1C60",
      "2027DD1B-2794-4B0A-B9DC-F7EE696411FF"
    ]
  }
}
```

```
HTTP/1.1 200 OK
Date: Fri, 08 Dec 2017 00:04:41 GMT
Content-Type: application/json;charset=UTF-8
Transfer-Encoding: chunked
{
  "data": {
    "promotedArticles": [
      "https://news-api.apple.com/articles/F59D1784-CAFC-432A-9A1A-EF2FCE1E1C60",
      "https://news-api.apple.com/articles/2027DD1B-2794-4B0A-B9DC-F7EE696411FF"
    ]
  }
}
```

## See Also

### Sections

List All Sections

See a list of available sections in your channel.

Read Section Information

Get information about the specified section, including its name, its channel, and whether it’s a default section.

object Section

See the fields the section endpoints returned.

object SectionLinks

See the links the section endpoints returned.

object SectionResponse

See which objects make up the section response.

object PromoteArticleRequest

See the required field for the Promote an Article request.

object PromoteArticleResponse

See the field the Promote an Article response returned.

