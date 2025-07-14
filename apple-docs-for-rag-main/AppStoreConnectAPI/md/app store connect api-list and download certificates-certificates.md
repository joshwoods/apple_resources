

- App Store Connect API
-  List and Download Certificates 

Web Service Endpoint

# List and Download Certificates

Find and list certificates and download their data.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/certificates
```

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `name, certificateType, displayName, serialNumber, platform, expirationDate, certificateContent, activated`

`filter[id]`

`[string]`

`filter[serialNumber]`

`[string]`

`limit`

`integer`

Maximum: `200`

`sort`

`[string]`

Possible Values: `displayName, -displayName, certificateType, -certificateType, serialNumber, -serialNumber, id, -id`

`filter[certificateType]`

`[string]`

Possible Values: `APPLE_PAY, APPLE_PAY_MERCHANT_IDENTITY, APPLE_PAY_PSP_IDENTITY, APPLE_PAY_RSA, DEVELOPER_ID_KEXT, DEVELOPER_ID_KEXT_G2, DEVELOPER_ID_APPLICATION, DEVELOPER_ID_APPLICATION_G2, DEVELOPMENT, DISTRIBUTION, IDENTITY_ACCESS, IOS_DEVELOPMENT, IOS_DISTRIBUTION, MAC_APP_DISTRIBUTION, MAC_INSTALLER_DISTRIBUTION, MAC_APP_DEVELOPMENT, PASS_TYPE_ID, PASS_TYPE_ID_WITH_NFC`

`filter[displayName]`

`[string]`

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

### Getting certificate infomation and data

Read and Download Certificate Information

Get information about a certificate and download the certificate data.

