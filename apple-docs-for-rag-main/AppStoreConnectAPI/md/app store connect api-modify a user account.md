

- App Store Connect API
-  Modify a User Account 

Web Service Endpoint

# Modify a User Account

Change a user’s role, app visibility information, or other account details.

App Store Connect API 1.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/users/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

UserUpdateRequest

Content-Type: application/json

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Modifying and Removing User Accounts

Remove a User Account

Remove a user from your team.

