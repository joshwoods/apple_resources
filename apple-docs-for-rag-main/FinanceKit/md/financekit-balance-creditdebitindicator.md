

- FinanceKit
- Balance
-  creditDebitIndicator 

Instance Property

# creditDebitIndicator

A value that indicates whether the balance is a credit or a debit balance.

iOS 17.4+iPadOS 17.4+

``` source
let creditDebitIndicator: CreditDebitIndicator
```

## Discussion

If an asset account has a positive balance, then the CreditDebitIndicator is CreditDebitIndicator.credit. If it has a negative balance, then the `CreditDebitIndicator` is CreditDebitIndicator.debit.

If a liability account has a *spent* balance, then the `CreditDebitIndicator` is `CreditDebitIndicator/debit`. If it has been *is in credit* then the `CreditDebitIndicator` is `CreditDebitIndicator/credit`.

Note

FinanceKit considers a zero balance to be a credit balance.

