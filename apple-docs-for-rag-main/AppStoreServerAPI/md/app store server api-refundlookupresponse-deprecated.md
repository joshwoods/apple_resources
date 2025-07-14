

- App Store Server API
-  RefundLookupResponse Deprecated

Object

# RefundLookupResponse

A response that contains an array of signed JSON Web Signature (JWS) transactions.

App Store Server API 1.1–1.6Deprecated

``` source
object RefundLookupResponse
```

Deprecated

Use Get Refund History and its response, RefundHistoryResponse, instead.

## Properties

`signedTransactions`

`[`JWSTransaction`]`

Deprecated 

A list of JWS transactions, or an empty array if the customer has received no refunds in your app. The transactions are sorted in ascending order by their revocationDate.

## Mentioned in 

App Store Server API changelog

## Discussion

If the customer hasn’t received any refunds for in-app purchases in your app, the `signedTransactions` array is empty. To read the transaction information, decode the payload for each JWSTransaction object in the `signedTransactions` array. Use a JWSTransactionDecodedPayload object to read the transaction information in the payload.

This response can contain a maximum of 50 transactions in the `signedTransactions` array.

## See Also

### Refund lookup

Get Refund History

Get a paginated list of all of a customer’s refunded in-app purchases for your app.

object RefundHistoryResponse

A response that contains an array of signed JSON Web Signature (JWS) refunded transactions, and paging information.

Get Refund History V1

Get a list of up to 50 of a customer’s refunded in-app purchases for your app.

Deprecated

