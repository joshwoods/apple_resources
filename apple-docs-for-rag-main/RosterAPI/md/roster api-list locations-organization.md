

- Roster API
-  List locations 

Web Service Endpoint

# List locations

Returns a list of locations in an Apple School Manager organization.

Roster API 1.0.0+

## URL

``` source
GET https://api-school.apple.com/rosterapi/v1/locations
```

## Query Parameters

`limit`

`string`

The maximum number of locations to return. The default is 100.

`pageToken`

`string`

A token for paging through a large number of results. If the number of locations in the organization is greater than the `limit` parameter, pass the token returned in Locations.

## Response Codes

` 200 ``OK`

Locations

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The access token was invalid.

` 403 ``Forbidden`

`Forbidden`

You don’t have permission to access the locations.

` 429 `

The client made too many requests. The response includes an `X-Retry-After` header that indicates the number of seconds to wait before making another request.

` 500 ``Internal Server Error`

`Internal Server Error`

The server encountered an internal error.

## Discussion

Access to the `locations` resource requires authorization to either the `edu.users.read` or `edu.classes.read` scope.

### Example

- Request
- Response

```
curl "https://api-school.apple.com/rosterapi/v1/locations?limit=1" -H "Authorization: Bearer ${TOKEN}"
```

```
{
  "locations":[{"id":"1234","name":"Example Location","domain":"example.com","timeZone":"PST","dateCreated":"2020-07-06T20:32:00Z","dateLastModified":"2023-04-20T09:49:33.938397143Z"}],
  "nextPageToken":"XbdJJGHGTqnueAVPfw2XOA",
  "moreToFollow":true
}
```

## See Also

### Information about locations

Read a location

Returns a specific location in an Apple School Manager organization.

object Location

A location in an Apple School Manager organization.

object Locations

A list of locations, with a token for pagination.

