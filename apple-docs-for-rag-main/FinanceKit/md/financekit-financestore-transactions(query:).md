

- FinanceKit
- FinanceStore
-  transactions(query:) 

Instance Method

# transactions(query:)

Returns transactions that match the provided transaction query.

iOS 17.4+iPadOS 17.4+

``` source
func transactions(query: TransactionQuery) async throws -> [Transaction]
```

## Parameters 

`query`  

A TransactionQuery that describes the kinds of transactions to look for.

## Return Value

An array of Transaction records that match the provided `query`.

## See Also

### Transactions

func transactionHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Transaction>

Returns the transactions for the specified account ID, optional starting time, and monitoring indicator for long running transaction queries.

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

