

- App Store Connect API
-  Revoke a Certificate 

Web Service Endpoint

# Revoke a Certificate

Revoke a lost, stolen, compromised, or expiring signing certificate.

App Store Connect API 1.1+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/certificates/{id}
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

## Mentioned in 

Managing merchant IDs and Payment Processing certificates

