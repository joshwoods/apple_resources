

- Apple Pay on the Web
- ApplePayShippingMethod
-  amount 

Instance Property

# amount

The nonnegative cost associated with this shipping method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString amount;
```

## Discussion

The amount must be nonnegative to pass validation.

## See Also

### Working with shipping method properties

label

A short description of the shipping method.

detail

Additional description of the shipping method.

dateComponentsRange

The expected range of dates for shipping or picking up an item.

identifier

A client-defined value used to identify this shipping method.

ApplePayDateComponentsRange

A dictionary that specifies the start and end dates for a range of time.

