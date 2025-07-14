

- App Store Connect API
-  Delete an End User License Agreement 

Web Service Endpoint

# Delete an End User License Agreement

Delete the custom end user license agreement that is associated with an app.

App Store Connect API 1.2+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Creating, Modifying, and Deleting an EULA

Create an End User License Agreement

Add a custom end user license agreement (EULA) to an app and configure the territories to which it applies.

Modify an End User License Agreement

Update the text or territories for your custom end user license agreement.

