

- PassKit (Apple Pay and Wallet)
-  PKAutomaticReloadPaymentSummaryItem 

Class

# PKAutomaticReloadPaymentSummaryItem

An object that defines a summary item for an automatic reload or refill payment, such as a store card top-up.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class PKAutomaticReloadPaymentSummaryItem
```

## Overview

PKAutomaticReloadPaymentSummaryItem is a subclass of PKPaymentSummaryItem and inherits all properties of the parent class.

Add a summary item of this type to the paymentSummaryItems property of a PKPaymentRequest object to display an automatic reload payment in the summary items on the payment sheet to the user.

To describe an automatic reload payment, set the summary item values as follows:

- Use the amount property to specify the reload amount when the account balance reaches the threshold amount, thresholdAmount.

- Omit the type property. The summary item type is only relevant for the PKPaymentSummaryItem parent class.

## Topics

### Setting the automatic reload threshold

var thresholdAmount: NSDecimalNumber

The balance an account reaches before you apply the automatic reload amount.

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

var automaticReloadBilling: PKAutomaticReloadPaymentSummaryItem

Summary items that contain the top-up amount and balance threshold amount for the automatic reload payment.

