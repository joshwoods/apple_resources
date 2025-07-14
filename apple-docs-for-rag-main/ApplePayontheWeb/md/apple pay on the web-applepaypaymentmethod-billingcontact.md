

- Apple Pay on the Web
- ApplePayPaymentMethod
-  billingContact 

Instance Property

# billingContact

The billing contact associated with the card.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayPaymentContact billingContact;
```

## Mentioned in 

Apple Pay on the Web Version 10 Release Notes

## Discussion

Before the user authorizes the transaction, you receive redacted billing contact information in a callback event. The redacted information includes only the necessary data for completing transaction tasks, such as calculating taxes or shipping costs.

## See Also

### Accessing payment method data

displayName

A string, suitable for display, that describes the card.

network

A string, suitable for display, that is the name of the payment network backing the card.

type

A string value representing the card’s type of payment.

paymentPass

The payment pass object currently selected to complete the payment.

