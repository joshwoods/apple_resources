

- Apple Pay on the Web
- ApplePayShippingContactUpdate
-  errors 

Instance Property

# errors

A list of custom errors to display on the payment sheet.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Desktop**

``` source
sequence  errors;
```

**Unsupported OS: Safari Mobile**

``` source
sequence  errors;
```

## Discussion

List the errors on the payment sheet for the user to remedy. If there are multiple errors, list the most important error first.

For information on errors, see ApplePayError.

## See Also

### Updating shipping contact properties

newLineItems

An optional list of updated line items.

newShippingMethods

A list of shipping methods that are available to the updated shipping contact.

newTotal

The new total that results from a change in the shipping contact.

