

- FinanceKit
- AccountBalanceQuery
-  predicate(availableSince:until:) 

Type Method

# predicate(availableSince:until:)

A predicate that returns available account balances since a specified date, and, optionally, until another date.

iOS 17.4+iPadOS 17.4+

``` source
static func predicate(
    availableSince startDate: Date,
    until endDate: Date? = nil
) -> Predicate
```

## Parameters 

`startDate`  

The date to start collecting account balances.

`endDate`  

The date to end collection account balances. This parameter is optional. If this parameter isn’t included, the method returns all account balances since the `startDate`.

