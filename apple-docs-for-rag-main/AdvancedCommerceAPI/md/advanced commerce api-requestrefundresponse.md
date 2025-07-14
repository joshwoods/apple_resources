

- Advanced Commerce API
-  RequestRefundResponse 

Object

# RequestRefundResponse

The response body for a transaction refund request.

Advanced Commerce API 1.1+

``` source
object RequestRefundResponse
```

## Properties

`signedRenewalInfo`

JWSRenewalInfo

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format.

`signedTransactionInfo`

JWSTransaction

 (Required) 

Transaction information signed by the App Store, in JWS Compact Serialization format.

## Overview

\##Discussion This is the response body for the Request Transaction Refund endpoint.

## See Also

### Refund request from the server

Request Transaction Refund

Request a refund for a one-time charge or subscription transaction.

object RequestRefundRequest

The request body for requesting a refund for a transaction.

object RequestRefundItem

Information about the refund request for an item, such as its SKU, the refund amount, reason, and type.

