

- PassKit (Apple Pay and Wallet)
-  PKRecurringPaymentSummaryItem 

Class

# PKRecurringPaymentSummaryItem

An object that defines a summary item for a payment that occurs repeatedly at a specified interval, such as a subscription.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class PKRecurringPaymentSummaryItem
```

## Overview

PKRecurringPaymentSummaryItem is a subclass of PKPaymentSummaryItemType and inherits all properties of the parent class.

Add a summary item of this type to the paymentSummaryItems property of a PKPaymentRequest to display to the user a recurring payment in the summary items on the payment sheet.

To describe a recurring payment, set the summary item values as follows:

- In the amount property, provide the billing amount for the set interval, for example, the amount charged per week if the intervalUnit is a week.

- Omit the type property. The summary item type is only relevant for the PKPaymentSummaryItem parent class.

- Set the startDate and endDate to represent the term for the recurring payments, as appropriate.

- Set the intervalUnit, intervalCount, and endDate to specify a number of repeating payments.

For example, the following code shows a summary item that specifies six monthly payments that start on the transaction date:

```
let recurringPayment = PKRecurringPaymentSummaryItem(label: "Total Payment",                                                  NSDecimalNumber(string: "199.99"))

// Payment starts today.
recurringPayment.startDate = nil

// Pay once a month.
recurringPayment.intervalUnit = .month
recurringPayment.intervalCount = 1

// Make 5 more payments for a total of 6 payments.
var dateComponent = DateComponents()
dateComponent.month = 5
recurringPayment.endDate = Calendar.current.date(byAdding: dateComponent, Date())
```

The payment interval is a combination of the intervalUnit and the intervalCount. For example, if you set the intervalUnit to .month and intervalCount to `3`, then the payment interval is three months.

## Topics

### Setting the payment period

var startDate: Date?

The date of the first payment.

var endDate: Date?

The date of the final payment.

### Setting the payment interval

var intervalUnit: NSCalendar.Unit

The amount of time – in calendar units such as day, month, or year – that represents a fraction of the total payment interval.

var intervalCount: Int

The number of interval units that make up the total payment interval.

## Relationships

### Inherits From

- PKPaymentSummaryItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Setting the payment summary items

var paymentSummaryItems: [PKPaymentSummaryItem]

An array of payment summary item objects that summarize the amount of the payment.

class PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

class PKDeferredPaymentSummaryItem

An object that defines a summary item for a payment that occurs at a later date, such as a pre-order.

