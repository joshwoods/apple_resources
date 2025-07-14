

- Enterprise Program API
-  List Users 

Web Service Endpoint

# List Users

Get a list of the users on your team.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/users
```

## Query Parameters

`fields[users]`

`[string]`

Fields to return for included related types.

Possible Values: `firstName, lastName, roles, username`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `lastName, -lastName, username, -username`

`filter[roles]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `ADMIN, ACCOUNT_HOLDER, DEVELOPER`

`filter[username]`

`[string]`

Attributes, relationships, and IDs by which to filter.

## Response Codes

` 200 ``OK`

UsersResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

### Example Request and Response

- Request
- Response

```
https://qa.api.adep.ase.apple.com/v1/users?limit=2
```

```
```

## See Also

### Getting User Information

Read User Information

Get information about a user on your team, such as name, roles, and app visibility.

