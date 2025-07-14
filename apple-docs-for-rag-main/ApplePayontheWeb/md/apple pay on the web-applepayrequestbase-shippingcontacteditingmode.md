

- Apple Pay on the Web
- ApplePayRequestBase
-  shippingContactEditingMode 

Instance Property

# shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayShippingContactEditingMode shippingContactEditingMode;
```

## Discussion

Set the value to `storePickup` for an in-store or other pickup to prevent the user from editing the shipping address.

For more information on configuring a package for store pickup, see Displaying a Read-Only Pickup Address.

Important

Determine whether to disable editing of the shipping contact field before displaying the payment sheet. Switching from a noneditable to an editable shipping contact field requires the user to restart the payment process.

## See Also

### Setting contact information

billingContact

A prepopulated billing address.

shippingContact

The customer’s address, used for sending products or services for to the person.

