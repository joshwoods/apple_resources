

- App Store Connect API
-  Create a merchant ID 

Web Service Endpoint

# Create a merchant ID

Add a new merchant ID to your team.

App Store Connect API 3.8+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/merchantIds
```

## HTTP Body

MerchantIdCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

MerchantIdResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

Managing merchant IDs and Payment Processing certificates

## See Also

### Managing merchant IDs

Managing merchant IDs and Payment Processing certificates

Create and update certificates so your app uses Apple Pay and Wallet.

List merchant IDs

List all merchant Ids for your team.

Read details for a merchant ID

Get information for a merchant ID.

List certificates for a merchant ID

Get a list of all certificates for a specific merchant ID.

Modify merchant IDs

Update a specific merchant ID.

Delete a merchant ID

Delete a specific merchant ID.

