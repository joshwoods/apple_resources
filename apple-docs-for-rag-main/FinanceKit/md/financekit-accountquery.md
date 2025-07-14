

- FinanceKit
-  AccountQuery 

Structure

# AccountQuery

A structure that defines an account query.

iOS 17.4+iPadOS 17.4+

``` source
struct AccountQuery
```

## Overview

Use an `AccountQuery` to find and filter a person’s accounts.

## Topics

### Initializers

init(sortDescriptors: [SortDescriptor&lt;Account>], predicate: Predicate&lt;Account>?, limit: Int?, offset: Int?)

Creates a new account query structure with the provided sort descriptors and, optionally, a predicate and limit on the number of records the query should return.

## Relationships

### Conforms To

- Sendable

## See Also

### Transactions

func transactionHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Transaction>

Returns the transactions for the specified account ID, optional starting time, and monitoring indicator for long running transaction queries.

func transactions(query: TransactionQuery) async throws -> [Transaction]

Returns transactions that match the provided transaction query.

struct AccountCreditInformation

A structure that describes the credit information associated with an account.

struct CurrencyAmount

A structure that describes a monetary amount and its currency.

struct Transaction

A structure that represents a transaction relating to a specific financial account.

struct TransactionQuery

A structure that describes the parameters to use for a transaction query.

enum TransactionType

Values that describe kinds of transactions.

enum TransactionStatus

Values that describe the status of a transaction.

