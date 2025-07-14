

- App Store Server API
-  TransactionInfoResponse 

Object

# TransactionInfoResponse

A response that contains signed transaction information for a single transaction.

App Store Server API 1.8+

``` source
object TransactionInfoResponse
```

## Properties

`signedTransactionInfo`

JWSTransaction

A customer’s in-app purchase transaction, signed by Apple, in JSON Web Signature (JWS) format.

## Mentioned in 

App Store Server API changelog

## Discussion

The `TransactionInfoResponse` contains information about the transaction that you request using the Get Transaction Info endpoint. The transactionId in the `signedTransactionInfo` matches the `transactionId` you provide in the request path.

## Topics

### Response data types

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

## See Also

### Transaction information

Get Transaction Info

Get information about a single transaction for your app.

