

- App Store Connect API
-  Modify a Bundle ID 

Web Service Endpoint

# Modify a Bundle ID

Update a specific bundle ID’s name.

App Store Connect API 1.1+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/bundleIds/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

BundleIdUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

BundleIdResponse

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

### Modifying and Removing Bundle IDs

Delete a Bundle ID

