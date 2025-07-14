

- Apple Pay on the Web
- ApplePayLineItem
-  recurringPaymentEndDate 

Instance Property

# recurringPaymentEndDate

The date of the final payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
Date recurringPaymentEndDate;
```

## Discussion

To specify no payment end date, don’t include this attribute.

## See Also

### Configuring recurring payments

recurringPaymentStartDate

The date of the first payment.

recurringPaymentIntervalUnit

The amount of time — in calendar units, such as day, month, or year — that represents a fraction of the total payment interval.

recurringPaymentIntervalCount

The number of interval units that make up the total payment interval.

ApplePayRecurringPaymentDateUnit

A type that indicates calendrical units, such as year, month, day, and hour.

