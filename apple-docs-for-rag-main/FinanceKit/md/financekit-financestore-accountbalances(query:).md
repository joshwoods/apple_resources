

- FinanceKit
- FinanceStore
-  accountBalances(query:) 

Instance Method

# accountBalances(query:)

Returns a list of balances that meet the criteria in the provided account query.

iOS 17.4+iPadOS 17.4+

``` source
func accountBalances(query: AccountBalanceQuery) async throws -> [AccountBalance]
```

## Parameters 

`query`  

An AccountQuery that describes the kinds of accounts to look for.

## Return Value

An array of AccountBalance structures.

## See Also

### Balances

func accountBalanceHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;AccountBalance>

Returns the account balance history since a time specified by the provided financial history token.

struct AccountBalance

A structure that describes the financial balance of an account at a specific point in time.

struct AccountBalanceQuery

A structure that defines an account balance query.

struct Balance

A structure that describes an account balance.

enum CreditDebitIndicator

Values that the framework uses to describe transactions as credits or debits.

enum CurrentBalance

Values that describe the state of an account’s credit balance.

