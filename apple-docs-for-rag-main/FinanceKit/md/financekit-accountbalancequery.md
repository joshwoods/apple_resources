

- FinanceKit
-  AccountBalanceQuery 

Structure

# AccountBalanceQuery

A structure that defines an account balance query.

iOS 17.4+iPadOS 17.4+

``` source
struct AccountBalanceQuery
```

## Overview

Use an `AccountBalanceQuery` to find and filter specific balances in a person’s accounts.

## Topics

### Initializers

init(sortDescriptors: [SortDescriptor&lt;AccountBalance>], predicate: Predicate&lt;AccountBalance>?, limit: Int?, offset: Int?)

Creates a new account balance query structure with the provided sort descriptors.

### Type Methods

static func predicate(availableSince: Date, until: Date?) -> Predicate&lt;AccountBalance>

A predicate that returns available account balances since a specified date, and, optionally, until another date.

static func predicate(bookedSince: Date, until: Date?) -> Predicate&lt;AccountBalance>

A predicate that returns booked account balances since a specified date until another date.

## Relationships

### Conforms To

- Sendable

## See Also

### Balances

func accountBalances(query: AccountBalanceQuery) async throws -> [AccountBalance]

Returns a list of balances that meet the criteria in the provided account query.

func accountBalanceHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;AccountBalance>

Returns the account balance history since a time specified by the provided financial history token.

struct AccountBalance

A structure that describes the financial balance of an account at a specific point in time.

struct Balance

A structure that describes an account balance.

enum CreditDebitIndicator

Values that the framework uses to describe transactions as credits or debits.

enum CurrentBalance

Values that describe the state of an account’s credit balance.

