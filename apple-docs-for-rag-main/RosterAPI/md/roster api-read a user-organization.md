

- Roster API
-  Read a user 

Web Service Endpoint

# Read a user

Read a user in an Apple School Manager organization.

Roster API 1.0.0+

## URL

``` source
GET https://api-school.apple.com/rosterapi/v1/users/{userId}
```

## Path Parameters

`userId`

`string`

 (Required) 

The identifier from the user. Use the `id` field from the User object.

## Response Codes

` 200 ``OK`

User

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

The server didn’t find a user with the given `userId` in the organization.

` 429 `

The client made too many requests. The response includes an `X-Retry-After` header that indicates the number of seconds to wait before making another request.

` 500 ``Internal Server Error`

`Internal Server Error`

The server encountered an internal error.

## Mentioned in 

Integrating with Roster API and Sign in with Apple

## Discussion

Access to the `users` resource requires authorization to the `edu.users.read` scope.

### Example

- Request
- Response

```
curl "https://api-school.apple.com/rosterapi/v1/users/1234" \
        -H "Authorization: Bearer ${TOKEN}"
```

```
{
  "id": "1234",
  "email": "user@example.edu",
  "givenName": "Finny",
  "middleName”: "Kim",
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
```

## See Also

### Information about users

object User

A user in an Apple School Manager organization.

object RoleLocation

A mapping between a role assumed by a user in an Apple School Manager organization, and the corresponding location.

List users

List users in an Apple School Manager organization.

List users in a class

List users in a class of an Apple School Manager organization.

object Users

A list of users, with a token for pagination.

