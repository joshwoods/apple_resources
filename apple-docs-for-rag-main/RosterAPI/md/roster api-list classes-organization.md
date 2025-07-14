

- Roster API
-  List classes 

Web Service Endpoint

# List classes

List classes in an Apple School Manager organization.

Roster API 1.0.0+

## URL

``` source
GET https://api-school.apple.com/rosterapi/v1/classes
```

## Query Parameters

`limit`

`string`

The maximum number of class records to return. The default is 100.

`pageToken`

`string`

A token for paging through a large number of results. If the number of records in the organization is greater than the `limit` parameter, pass the token returned in Classes.

## Response Codes

` 200 ``OK`

Classes

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The access token was invalid.

` 403 ``Forbidden`

`Forbidden`

Access to the list of classes was forbidden.

` 429 `

The client made too many requests. The response includes an `X-Retry-After` header that indicates the number of seconds to wait before making another request.

` 500 ``Internal Server Error`

`Internal Server Error`

The server encountered an internal error.

## Mentioned in 

Obtaining information about people and classes

## Discussion

### Example

- Request
- Response

```
curl "https://api-school.apple.com/rosterapi/v1/classes?limit=1" \
    -H "Authorization: Bearer ${ACCESS_TOKEN}"

```

```
```

## See Also

### Information about classes

Read a class

Read a class from an Apple School Manager organization.

object Class

A class in an Apple School Manager organization.

object Classes

A list of classes, with a token for pagination.

