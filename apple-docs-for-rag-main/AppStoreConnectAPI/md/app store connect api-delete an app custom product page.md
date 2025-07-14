

- App Store Connect API
-  Delete an app custom product page 

Web Service Endpoint

# Delete an app custom product page

Delete metadata that you configured for a custom product page.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appCustomProductPages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page resource ID from the List all custom product pages for an app response.

## Response Codes

` 204 ``No Content`

`No Content`

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/appCustomProductPages/eb2b3606-2fef-4aab-a54e-b2e5547c9bc3
```

```
204
```

## See Also

### Endpoints

Create a custom product page

Add a custom product page for your app.

Modify an app custom product page

Update the name and visibility status of an app custom product page.

List all custom product pages for an app

Get a list of all custom product pages for a specific app.

Read custom product page information

Get information about a specific app custom product page.

List custom product page versions

List the versions for a custom product page version.

