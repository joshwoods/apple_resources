

- Roster API
-  Read the organization 

Web Service Endpoint

# Read the organization

Returns information about the Apple School Manager organization.

Roster API 1.0.0+

## URL

``` source
GET https://api-school.apple.com/rosterapi/v1/organization
```

## Response Codes

` 200 ``OK`

Organization

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The access token was invalid.

` 403 ``Forbidden`

`Forbidden`

You don’t have permission to access the organization information.

` 404 ``Not Found`

`Not Found`

The server didn’t find the organization information.

` 429 `

The client made too many requests. The response includes an `X-Retry-After` header that indicates the number of seconds to wait before making another request.

` 500 ``Internal Server Error`

`Internal Server Error`

The server encountered an internal error.

## Mentioned in 

Integrating with Roster API and Sign in with Apple

## Discussion

Access to the `organization` resource requires authorization to either the `edu.users.read` or `edu.classes.read` scope.

### Example

- Request
- Response

```
curl "https://api-school.apple.com/rosterapi/v1/organization" -H "Authorization: Bearer ${TOKEN}"
```

```
{
  "id":"1234",
  "type":"EDUCATION",
  "name":"Example Organization",
  "domains":[{"name":"example.com","isVerified":false}],
  "dateCreated":"2022-10-11T01:53:02Z",
  "dateLastModified":"2022-10-11T01:53:02Z"
}
```

## See Also

### Information about the organization

object Organization

Information about an Apple School Manager organization.

object Domain

A DNS domain name associated with an Apple School Manager organization.

