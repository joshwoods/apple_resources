

- Enterprise Program API
-  Read and Download Certificate Information 

Web Service Endpoint

# Read and Download Certificate Information

Get information about a certificate and download the certificate data.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/certificates/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `certificateContent, certificateType, csrContent, displayName, expirationDate, name, passTypeId, platform, serialNumber`

`fields[passTypeIds]`

`[string]`

Possible Values: `certificates, identifier, name`

`include`

`[string]`

Value: `passTypeId`

## Response Codes

` 200 ``OK`

CertificateResponse

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

## See Also

### Getting Certificate Infomation and Data

List and Download Certificates

Find and list certificates and download their data.

