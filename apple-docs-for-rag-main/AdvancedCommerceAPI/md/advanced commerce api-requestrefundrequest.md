

- Advanced Commerce API
-  RequestRefundRequest 

Object

# RequestRefundRequest

The request body for requesting a refund for a transaction.

Advanced Commerce API 1.1+

``` source
object RequestRefundRequest
```

## Properties

`currency`

currency

The currency of the transaction.

`items`

`[`RequestRefundItem`]`

 (Required) 

`refundRiskingPreference`

refundRiskingPreference

 (Required) 

`requestInfo`

RequestInfo

 (Required) 

`storefront`

storefront

## Discussion

This is the request body for the Request Transaction Refund endpoint.

## See Also

### Refund request from the server

Request Transaction Refund

Request a refund for a one-time charge or subscription transaction.

object RequestRefundResponse

The response body for a transaction refund request.

object RequestRefundItem

Information about the refund request for an item, such as its SKU, the refund amount, reason, and type.

