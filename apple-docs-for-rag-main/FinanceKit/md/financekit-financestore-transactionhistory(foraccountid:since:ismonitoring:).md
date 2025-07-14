

- FinanceKit
- FinanceStore
-  transactionHistory(forAccountID:since:isMonitoring:) 

Instance Method

# transactionHistory(forAccountID:since:isMonitoring:)

Returns the transactions for the specified account ID, optional starting time, and monitoring indicator for long running transaction queries.

iOS 17.4+iPadOS 17.4+

``` source
func transactionHistory(
    forAccountID accountID: UUID,
    since token: FinanceStore.HistoryToken? = nil,
    isMonitoring: Bool = true
) -> FinanceStore.History
```

## Parameters 

`accountID`  

An account identifier.

`isMonitoring`  

A Boolean value that indicates the method should return records asynchronously as the system updates the FinanceStore.

## Return Value

A FinanceStore.History of transactions that match the provided `accountID`.

## Discussion

Use this method to search the finance store for transactions in a specific account and receive updates as the framework enters new transactions into the finance store. You can, optionally, specify a starting date and time by providing a `historyToken`.

## See Also

### Transactions

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

struct TransactionQuery

A structure that describes the parameters to use for a transaction query.

enum TransactionType

Values that describe kinds of transactions.

enum TransactionStatus

Values that describe the status of a transaction.

