

- Enterprise Program API
-  List and Download Certificates 

Web Service Endpoint

# List and Download Certificates

Find and list certificates and download their data.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/certificates
```

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `certificateContent, certificateType, csrContent, displayName, expirationDate, name, passTypeId, platform, serialNumber`

`fields[passTypeIds]`

`[string]`

Possible Values: `certificates, identifier, name`

`filter[certificateType]`

`[string]`

Possible Values: `IOS_DEVELOPMENT, IOS_DISTRIBUTION, MAC_APP_DISTRIBUTION, MAC_INSTALLER_DISTRIBUTION, MAC_APP_DEVELOPMENT, DEVELOPER_ID_KEXT, DEVELOPER_ID_APPLICATION, DEVELOPMENT, DISTRIBUTION, PASS_TYPE_ID, PASS_TYPE_ID_WITH_NFC`

`filter[displayName]`

`[string]`

`filter[id]`

`[string]`

`filter[serialNumber]`

`[string]`

`include`

`[string]`

Value: `passTypeId`

`limit`

`integer`

Maximum: `200`

`sort`

`[string]`

Possible Values: `certificateType, -certificateType, displayName, -displayName, id, -id, serialNumber, -serialNumber`

## Response Codes

` 200 ``OK`

CertificatesResponse

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

## See Also

### Getting Certificate Infomation and Data

Read and Download Certificate Information

Get information about a certificate and download the certificate data.

