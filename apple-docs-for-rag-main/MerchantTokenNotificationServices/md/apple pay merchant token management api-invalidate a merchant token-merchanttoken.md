

- Apple Pay Merchant Token Management API
-  Invalidate a Merchant Token 

Web Service Endpoint

# Invalidate a Merchant Token

Invalidate a merchant token associated with your merchant identifier, making it invalid for future transaction authorizations.

App Store Connect API 1.0.10+

## URL

``` source
POST https://apple-pay-gateway.apple.com/paymentservices/v1/merchantId/{merchantId}/merchantToken/unlink
```

## Path Parameters

`merchantId`

`string`

 (Required) 

Your merchant identifier.

## Header Parameters

`Accept`

`string`

`Content-Type`

`string`

 (Required) 

`x-request-id`

`string`

 (Required) 

## HTTP Body

MerchantTokenUnlinkRequest

The request body you use to specify the merchant token that Apple Pay should invalidate.

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

Success. The service doesn’t return any additional information.

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Invalid request. The merchant token identifier isn’t valid for the merchant identifier.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

Internal server error.

Content-Type: application/json

## Discussion

When you call this endpoint, Apple Pay server unlinks — invalidates — the merchant token, and the token is no longer valid for future transaction authorizations. Call this endpoint in the following cases:

- Someone cancels a recurring transaction on your website or in your app that uses this merchant token

- Someone changes the payment method for a recurring transactions, for example, they stop using Apple Pay for the transaction

## See Also

### Merchant token invalidation

object MerchantTokenUnlinkRequest

The request body you use to invalidate a merchant token.

