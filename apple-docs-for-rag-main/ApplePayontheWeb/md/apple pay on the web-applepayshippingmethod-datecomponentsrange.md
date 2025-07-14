

- Apple Pay on the Web
- ApplePayShippingMethod
-  dateComponentsRange 

Instance Property

# dateComponentsRange

The expected range of dates for shipping or picking up an item.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayDateComponentsRange dateComponentsRange;
```

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

## Discussion

Use this object to set the expected date range for shipping a package, or the time an item is available for pickup. The payment sheet displays the range as part of the shipping method on the main sheet. When assembling the date components, provide absolute dates to represent the range.

The example code below shows setting a two day time range for shipping a package that starts three days from today:

```
let shippingStart = new Date;
shippingStart.setDate(shippingStart.getDate() + 3);

let shippingEnd = new Date;
shippingEnd.setDate(shippingEnd.getDate() + 5);

let applePayShippingMethod = {
    amount: "0.00",
    dateComponentsRange: {
        startDateComponents: {
            year: shippingStart.getFullYear(),
            // Because the JavaScript getMonth() function is 0-based, add 1 to return a 1-based month.
            months: shippingStart.getMonth() + 1,
            days: shippingStart.getDate(),
        },
        endDateComponents: {
            year: shippingEnd.getFullYear(),
            months: shippingEnd.getMonth() + 1,
            days: shippingEnd.getDate(),
        },
    },
    detail: "Tickets sent to your address",
    identifier: "delivery",
    label: "Delivery",
};
```

## See Also

### Working with shipping method properties

label

A short description of the shipping method.

detail

Additional description of the shipping method.

identifier

A client-defined value used to identify this shipping method.

amount

The nonnegative cost associated with this shipping method.

ApplePayDateComponentsRange

A dictionary that specifies the start and end dates for a range of time.

