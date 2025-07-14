

- FinanceKit
- AccountCreditInformation
-  overduePaymentAmount 

Instance Property

# overduePaymentAmount

The amount by which the account is overdue for the current period.

iOS 17.4+iPadOS 17.4+

``` source
let overduePaymentAmount: CurrencyAmount?
```

## Discussion

If not `nil` and `minimumNextPaymentAmount` is not `nil` then the `minimumNextPaymentAmount` has information about the next bill.

