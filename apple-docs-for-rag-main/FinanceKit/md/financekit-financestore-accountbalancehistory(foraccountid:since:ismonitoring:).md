

- FinanceKit
- FinanceStore
-  accountBalanceHistory(forAccountID:since:isMonitoring:) 

Instance Method

# accountBalanceHistory(forAccountID:since:isMonitoring:)

Returns the account balance history since a time specified by the provided financial history token.

iOS 17.4+iPadOS 17.4+

``` source
func accountBalanceHistory(
    forAccountID accountID: UUID,
    since token: FinanceStore.HistoryToken? = nil,
    isMonitoring: Bool = true
) -> FinanceStore.History
```

## Parameters 

`accountID`  

A UUID that identifies a specific account a person has added to the finance store.

`isMonitoring`  

A Boolean value that indicates whether the framework should return a `History` sequence that indicates the changes to the accounts over time. Defaults to `true`.

## Discussion

Use this method to monitor the balance of a specific account. Provide a `historyToken` to specify a starting data and time.

## See Also

### Balances

func accountBalances(query: AccountBalanceQuery) async throws -> [AccountBalance]

Returns a list of balances that meet the criteria in the provided account query.

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

