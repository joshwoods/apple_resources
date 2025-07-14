

- Apple Pay on the Web
-  ApplePayLineItem 

Structure

# ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayLineItem {
 ApplePayLineItemType type;
 DOMString label;
 DOMString amount;
 ApplePayPaymentTiming paymentTiming;
 Date recurringPaymentStartDate;
 ApplePayRecurringPaymentDateUnit recurringPaymentIntervalUnit;
 long recurringPaymentIntervalCount;
 Date recurringPaymentEndDate;
 Date deferredPaymentDate;
 DOMString automaticReloadPaymentThresholdAmount;
};
```

## Overview

Line items appear in the payment sheet.

The following code is an example of a line item for a \$20 charge that recurs every six months starting on 01/01/2022 and ending on 01/01/2024:

```
{
    "label": "Subscription",
    "amount": "20.00",
    "type": "final",
    "paymentTiming": "recurring",
    "recurringPaymentStartDate": new Date("2022-01-01T00:00:00"),
    "recurringPaymentIntervalUnit": "month",
    "recurringPaymentIntervalCount": 6,
    "recurringPaymentEndDate": new Date("2024-01-01T00:00:00"),
}
```

The following code is an example of a line item for a deferred charge of \$50 on 07/01/2023:

```
{
    "label": "After Trial Period",
    "amount": "50.00",
    "type": "final",
    "paymentTiming": "deferred",
    "deferredPaymentDate": new Date("2023-07-01T00:00:00"),
}
```

For examples of line items within an ApplePayPaymentRequest, see lineItems and total.

## Topics

### Setting line item properties

label

A required value that’s a short, localized description of the line item.

amount

A required value that’s the monetary amount of the line item.

type

A value that indicates whether the line item is final or pending.

### Configuring payment timing

paymentTiming

The time that the payment occurs as part of a successful transaction.

ApplePayPaymentTiming

A type that indicates the time a payment occurs in a transaction.

### Configuring recurring payments

recurringPaymentStartDate

The date of the first payment.

recurringPaymentEndDate

The date of the final payment.

recurringPaymentIntervalUnit

The amount of time — in calendar units, such as day, month, or year — that represents a fraction of the total payment interval.

recurringPaymentIntervalCount

The number of interval units that make up the total payment interval.

ApplePayRecurringPaymentDateUnit

A type that indicates calendrical units, such as year, month, day, and hour.

### Configuring deferred payments

deferredPaymentDate

The date, in the future, of the payment.

### Configuring automatic reload payments

automaticReloadPaymentThresholdAmount

The balance an account reaches before the merchant applies the automatic reload amount.

## See Also

### Setting the total and summary line items

total

A line item that represents the total for the payment.

lineItems

A set of line items that explain recurring payments and additional charges and discounts.

ApplePayLineItemType

A type that indicates whether a line item is final or pending.

