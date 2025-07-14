

- App Store Connect API
-  List merchant IDs 

Web Service Endpoint

# List merchant IDs

List all merchant Ids for your team.

App Store Connect API 3.8+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/merchantIds
```

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `name, certificateType, displayName, serialNumber, platform, expirationDate, certificateContent, activated`

`fields[merchantIds]`

`[string]`

Possible Values: `name, identifier, certificates`

`filter[identifier]`

`[string]`

`filter[name]`

`[string]`

`include`

`[string]`

Value: `certificates`

`limit`

`integer`

Maximum: `200`

`limit[certificates]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `name, -name, identifier, -identifier`

## Response Codes

` 200 ``OK`

MerchantIdsResponse

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

## See Also

### Managing merchant IDs

Managing merchant IDs and Payment Processing certificates

Create and update certificates so your app uses Apple Pay and Wallet.

Read details for a merchant ID

Get information for a merchant ID.

List certificates for a merchant ID

Get a list of all certificates for a specific merchant ID.

Modify merchant IDs

Update a specific merchant ID.

Create a merchant ID

Add a new merchant ID to your team.

Delete a merchant ID

Delete a specific merchant ID.

