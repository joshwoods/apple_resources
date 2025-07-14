

- Apple Pay on the Web
- ApplePayPaymentToken
-  paymentData 

Instance Property

# paymentData

An object containing the encrypted payment data.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
JSON paymentData;
```

## Discussion

This data is used by your e-commerce back-end system, which decrypts it and submits it to your payment processor.

For the format of the payment data, see Payment token format reference.

## See Also

### Payment Token Properties

paymentMethod

Information about the card used in the transaction.

transactionIdentifier

A unique identifier for this payment.

