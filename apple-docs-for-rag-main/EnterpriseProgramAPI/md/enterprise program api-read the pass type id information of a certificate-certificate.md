

- Enterprise Program API
-  Read the Pass Type Id Information of a Certificate 

Web Service Endpoint

# Read the Pass Type Id Information of a Certificate

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/certificates/{id}/passTypeId
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

Value: `certificates`

`limit[certificates]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

PassTypeIdResponse

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

