

- FinanceKit
-  TransactionQuery 

Structure

# TransactionQuery

A structure that describes the parameters to use for a transaction query.

iOS 17.4+iPadOS 17.4+

``` source
struct TransactionQuery
```

## Overview

Use a `TransactionQuery` to find and filter transactions in a person’s accounts.

## Topics

### Initializers

init(sortDescriptors: [SortDescriptor&lt;Transaction>], predicate: Predicate&lt;Transaction>?, limit: Int?, offset: Int?)

Creates a new transaction query with the provided sort descriptors, predicate, and limit on the number of records the query should return.

### Type Methods

static func predicate(forMerchantCategoryCodes: [MerchantCategoryCode]) -> Predicate&lt;Transaction>

A predicate that returns transactions that match any of the provided merchant category codes.

static func predicate(forStatuses: [TransactionStatus]) -> Predicate&lt;Transaction>

Returns a predicate that matches any of the provided transaction statuses.

static func predicate(forTransactionTypes: [TransactionType]) -> Predicate&lt;Transaction>

Returns a predicate that matches any of the provided transaction types.

## Relationships

### Conforms To

- Sendable

## See Also

### Transactions

func transactionHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Transaction>

Returns the transactions for the specified account ID, optional starting time, and monitoring indicator for long running transaction queries.

func transactions(query: TransactionQuery) async throws -> [Transaction]

Returns transactions that match the provided transaction query.

struct AccountQuery

A structure that defines an account query.

struct AccountCreditInformation

A structure that describes the credit information associated with an account.

struct CurrencyAmount

A structure that describes a monetary amount and its currency.

struct Transaction

A structure that represents a transaction relating to a specific financial account.

enum TransactionType

Values that describe kinds of transactions.

enum TransactionStatus

Values that describe the status of a transaction.

