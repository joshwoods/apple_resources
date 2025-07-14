

- Enterprise Program API
-  Read User Information 

Web Service Endpoint

# Read User Information

Get information about a user on your team, such as name, roles, and app visibility.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/users/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[users]`

`[string]`

Fields to return for included related types.

Possible Values: `firstName, lastName, roles, username`

## Response Codes

` 200 ``OK`

UserResponse

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

### Example Request and Response

- Request
- Response

```
https://qa.api.adep.ase.apple.com/v1/users/345bb7dc-a653-43ff-acee-a4817cd28479
```

```
{
"data": {
"type": "users",
"id": "345bb7dc-a653-43ff-acee-a4817cd28479",
"attributes": {
"username": "ifuko+6env3@apple.com",
"firstName": "Ildiko",
"lastName": "Ln6Env3",
"roles": [
"ADMIN"
]
},
"links": {
"self": "https://qa.api.adep.ase.apple.com/v1/users/345bb7dc-a653-43ff-acee-a4817cd28479"
}
},
"links": {
"self": "https://qa.api.adep.ase.apple.com/v1/users/345bb7dc-a653-43ff-acee-a4817cd28479"
}
}
```

## See Also

### Getting User Information

List Users

Get a list of the users on your team.

