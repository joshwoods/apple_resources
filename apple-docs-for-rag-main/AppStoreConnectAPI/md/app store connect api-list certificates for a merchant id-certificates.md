

- App Store Connect API
-  List certificates for a merchant ID 

Web Service Endpoint

# List certificates for a merchant ID

Get a list of all certificates for a specific merchant ID.

App Store Connect API 3.8+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/merchantIds/{id}/certificates
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the merchant ID resource ID from the List merchant IDs response.

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `name, certificateType, displayName, serialNumber, platform, expirationDate, certificateContent, activated`

`filter[certificateType]`

`[string]`

Possible Values: `APPLE_PAY, APPLE_PAY_MERCHANT_IDENTITY, APPLE_PAY_PSP_IDENTITY, APPLE_PAY_RSA, DEVELOPER_ID_KEXT, DEVELOPER_ID_KEXT_G2, DEVELOPER_ID_APPLICATION, DEVELOPER_ID_APPLICATION_G2, DEVELOPMENT, DISTRIBUTION, IDENTITY_ACCESS, IOS_DEVELOPMENT, IOS_DISTRIBUTION, MAC_APP_DISTRIBUTION, MAC_INSTALLER_DISTRIBUTION, MAC_APP_DEVELOPMENT, PASS_TYPE_ID, PASS_TYPE_ID_WITH_NFC`

`filter[displayName]`

`[string]`

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

## Response Codes

` 200 ``OK`

CertificatesResponse

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

## See Also

### Managing merchant IDs

Managing merchant IDs and Payment Processing certificates

Create and update certificates so your app uses Apple Pay and Wallet.

List merchant IDs

List all merchant Ids for your team.

Read details for a merchant ID

Get information for a merchant ID.

Modify merchant IDs

Update a specific merchant ID.

Create a merchant ID

Add a new merchant ID to your team.

Delete a merchant ID

Delete a specific merchant ID.

