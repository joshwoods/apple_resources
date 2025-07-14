

- Apple Pay on the Web
- ApplePayRequestBase
-  shippingContact 

Instance Property

# shippingContact

The customer’s address, used for sending products or services for to the person.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayPaymentContact shippingContact;
```

## Discussion

If you have an up-to-date shipping address on file for the customer, you can set it here. See ApplePayPaymentContact for the fields in shippingContact.

The payment sheet displays the information you provide in shippingContact as the default shipping address. The user can either keep the address you provide or select another address.

Provide your user’s shipping contact info only if you request shipping information by setting `requestShipping` to `true` in your PaymentOptions dictionary.

## See Also

### Setting contact information

billingContact

A prepopulated billing address.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

