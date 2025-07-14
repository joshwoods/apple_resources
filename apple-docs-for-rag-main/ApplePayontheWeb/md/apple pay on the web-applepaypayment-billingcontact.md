

- Apple Pay on the Web
- ApplePayPayment
-  billingContact 

Instance Property

# billingContact

The billing contact selected by the user for this transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayPaymentContact billingContact;
```

## Discussion

The billing contact information is populated if it is requested in ApplePayPaymentRequest.

After the user authorizes the transaction with Touch ID, Face ID, or passcode, `billingContact` contains the complete billing contact data. See ApplePayPaymentContact for the billing contact field values.

Note

Address information can come from a wide range of sources. Always validate the information before you use it.

## See Also

### Billing and shipping contacts

shippingContact

The shipping contact selected by the user for this transaction.

ApplePayPaymentContact

Contact information fields to use for billing and shipping contact information.

