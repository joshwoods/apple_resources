

- App Store Connect API
-  Modify a certificate 

Web Service Endpoint

# Modify a certificate

Update the activation status for a specific certificate.

App Store Connect API 3.8+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/certificates/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List and Download Certificates response.

## HTTP Body

CertificateUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

CertificateResponse

`OK`

Content-Type: application/json

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

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

Managing merchant IDs and Payment Processing certificates

App Store Connect API 3.8 release notes

## See Also

### Creating and modifying certificates

Create a Certificate

Create a new certificate using a certificate signing request.

