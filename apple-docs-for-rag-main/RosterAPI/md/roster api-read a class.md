

- Roster API
-  Read a class 

Web Service Endpoint

# Read a class

Read a class from an Apple School Manager organization.

Roster API 1.0.0+

## URL

``` source
GET https://api-school.apple.com/rosterapi/v1/classes/{classId}
```

## Path Parameters

`classId`

`string`

 (Required) 

The identifier from the class. Use the `id` field from the Class object.

## Response Codes

` 200 ``OK`

Class

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The access token was invalid.

` 403 ``Forbidden`

`Forbidden`

Access to the requested class was forbidden.

` 404 ``Not Found`

`Not Found`

The server didn’t find a class with the given `classId` in the organization.

` 429 `

The client made too many requests. The response includes an `X-Retry-After` header that indicates the number of seconds to wait before making another request.

` 500 ``Internal Server Error`

`Internal Server Error`

The server encountered an internal error.

## Discussion

### Example

- Request
- Response

```
curl "https://api-school.apple.com/rosterapi/v1/classes/1234" \
    -H "Authorization: Bearer ${TOKEN}"
```

```
{
  "id": "1234",
  "name": "Algebra",
  "number": "101",
  "room": "PL-213",
  "locationId": "LO:1234",
  "instructorIds": [
    "1234",
    "2345"
  ],
  "studentIds": [
    "54321",
    "54322",
    "54323"
  ],
  "dateCreated": "2021-07-26T11:11:51Z",
  "dateLastModified”: "2021-07-26T11:11:51Z"
}
```

## See Also

### Information about classes

object Class

A class in an Apple School Manager organization.

List classes

List classes in an Apple School Manager organization.

object Classes

A list of classes, with a token for pagination.

