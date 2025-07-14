

- Apple News API
-  Read Section Information 

Web Service Endpoint

# Read Section Information

Get information about the specified section, including its name, its channel, and whether it’s a default section.

Apple News API 1.0+

## URL

``` source
GET https://news-api.apple.com/sections/{sectionId}
```

## Path Parameters

`sectionId`

`string`

 (Required) 

The UUID of the section with information to fetch.

## Response Codes

` 200 ``OK`

SectionResponse

`OK`

The request was successful.

Content-Type: application/json

` 400 ``Bad Request`

Error

`Bad Request`

- `MISSING.` You didn’t include the section UUID field in the request. Key path: `sectionid`.

- `INVALID_TYPE`. The value you specified for the section is not of the correct type for that field. Key path: `sectionid`.

Content-Type: application/json

` 401 ``Unauthorized`

Error

`Unauthorized`

You didn’t include the `Authorization` header. Key path: None.

Content-Type: application/json

` 403 ``Forbidden`

Error

`Forbidden`

You tried to access a channel your API key doesn’t have permission to access. Key path: None.

Content-Type: application/json

` 404 ``Not Found`

Error

`Not Found`

- The endpoint you tried to access doesn’t exist. Key path: None.

- The section you tried to access doesn’t exist. Key path: `sectionId`.

Content-Type: application/json

## Discussion

A Read Section Information request retrieves information about a single section. A section is a grouping of articles on a particular topic; for example, Sports, Silicon Valley, or Politics.

Every channel has a default section, even if no other sections are defined. See Add and manage sections in News Publisher User Guide.

### Example

- Request
- Response

```
GET /sections/4523e2f6-89fb-4842-b9f2-46514f7ebc6b HTTP/1.1
Host: news-api.apple.com
Accept: application/json
Authorization: HHMAC; key="1e3gfc5e-e9f8-4232-a6be-17bf40edad09"; signature="mLtpym3Lgl1300t8cze9wyWOaxkRBKL3j3ztalMjgWs="; date="2015-03-05T02:49:58Z"
```

```
HTTP/1.1 200 OK
Date: Thu, 05 Mar 2015 02:53:54 GMT
Content-Type: application/json;charset=UTF-8
Transfer-Encoding: chunked
{
  "data": {
    "createdAt": "2015-03-05T02:49:58Z",
    "modifiedAt": "2015-03-05T02:49:58Z",
    "id": "4523e2f6-89fb-4842-b9f2-46514f7ebc6b",
    "type": "section",
    "shareUrl": "https://apple.news/ArRPpLPE9QXu3sehS0rvxvA",
    "links": {
      "channel": "https://news-api.apple.com/channels/a5164537-3f2e-3569-8ff4-d5ac865e520e",
      "self": "https://news-api.apple.com/sections/4523e2f6-89fb-4842-b9f2-46514f7ebc6b"
    },
    "name": "Business",
    "isDefault": false
  }
}
```

## See Also

### Sections

List All Sections

See a list of available sections in your channel.

Promote Articles in a Section

Set the list of promoted articles for the specified section.

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

