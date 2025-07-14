

- Roster API
-  List users in a class 

Web Service Endpoint

# List users in a class

List users in a class of an Apple School Manager organization.

Roster API 1.0.0+

## URL

``` source
GET https://api-school.apple.com/rosterapi/v1/classes/{classId}/users
```

## Path Parameters

`classId`

`string`

 (Required) 

A unique class identifier. Use an identifier from the `id` field of Class.

## Query Parameters

`limit`

`string`

The maximum number of user records to return. The default limit is 100.

`role`

`string`

The role of the user in the class.

Possible Values: `Student, Instructor`

`pageToken`

`string`

A token to retrieve the next set of records when the number of users is greater than the `limit` parameter.

## Response Codes

` 200 ``OK`

Users

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The access token was invalid.

` 403 ``Forbidden`

`Forbidden`

Access to the requested user was forbidden.

` 404 ``Not Found`

`Not Found`

The server didn’t find a class with the given `classId` in the organization.

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
curl "https://api-school.apple.com/rosterapi/v1/classes/1234/users?role=Student&limit=1" \
    -H "Authorization: Bearer ${ACCESS_TOKEN}"
```

```
{
  "users": [
    {
      "id": "1234",
      "email": "user@example.edu",
      "givenName": "Finny",
      "middleName": "Kim",
      "familyName": "Ho",
      "grade": "10",
      "roleLocationMapping": [
        {
          "roleName": "Student",
          "locationId": "LO:1234"
        }
      ],
      "dateCreated": "2022-04-25T16:00:45Z",
      "dateLastModified": "2022-04-25T16:00:45Z"
    }
  ],
  "moreToFollow": true,
  "nextPageToken": "3da541559918a808c2402bba5012f6c60b27661c"
}
```

## See Also

### Information about users

Read a user

Read a user in an Apple School Manager organization.

object User

A user in an Apple School Manager organization.

object RoleLocation

A mapping between a role assumed by a user in an Apple School Manager organization, and the corresponding location.

List users

List users in an Apple School Manager organization.

object Users

A list of users, with a token for pagination.

