

- App Store Connect API
-  Modify merchant IDs 

Web Service Endpoint

# Modify merchant IDs

Update a specific merchant ID.

App Store Connect API 3.8+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/merchantIds/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the merchant ID resource ID from the List merchant IDs response.

## HTTP Body

MerchantIdUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

MerchantIdResponse

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

Create a merchant ID

Add a new merchant ID to your team.

Delete a merchant ID

Delete a specific merchant ID.

