

- Apple Pay Merchant Token Management API
-  Get Details of a Merchant Token Event 

Web Service Endpoint

# Get Details of a Merchant Token Event

Get the details of a merchant token event after receiving a notification.

App Store Connect API 1.0.10+

## URL

``` source
GET https://apple-pay-gateway.apple.com/paymentservices/v1/merchantId/{merchantId}/merchantToken/event/{eventId}
```

## Path Parameters

`eventId`

`string`

 (Required) 

A unique event identifier that you receive in a notification from the Apple Pay server.

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

## Response Codes

` 200 ``OK`

MerchantTokenEventResponse

`OK`

Successful response.

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Bad request.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

Internal server error.

Content-Type: application/json

## Discussion

For information about setting your server’s notification URL to receive life-cycle events, see tokenNotificationURL in PKAutomaticReloadPaymentRequest, tokenNotificationURL in PKRecurringPaymentRequest, tokenNotificationURL in ApplePayAutomaticReloadPaymentRequest, or tokenNotificationURL in ApplePayRecurringPaymentRequest.

## See Also

### Merchant token event retrieval

object MerchantTokenEventResponse

A response body that contains information about a life-cycle event for a merchant token.

object MerchantTokenMetadata

The card information related to a merchant token, including its card art and metadata.

object CardArt

Data for displaying art to represent a card.

object CardMetadata

Data about the card, including its expiration date and suffix.

