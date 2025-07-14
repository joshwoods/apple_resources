

- Apple Pay on the Web
-  ApplePayDateComponentsRange 

Structure

# ApplePayDateComponentsRange

A dictionary that specifies the start and end dates for a range of time.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayDateComponentsRange {
 required ApplePayDateComponents startDateComponents;
 required ApplePayDateComponents endDateComponents;
};
```

## Topics

### Start and End Dates of the Range

startDateComponents

The start date and time of the range.

endDateComponents

The end date and time of the range.

ApplePayDateComponents

A dictionary that specifies the values for the calendrical units for a date.

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

amount

The nonnegative cost associated with this shipping method.

