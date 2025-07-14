

- FinanceKit
- FinanceStore
-  accounts(query:) 

Instance Method

# accounts(query:)

Returns a list of accounts a person added to their Wallet that meet the criteria in the provided account query.

iOS 17.4+iPadOS 17.4+

``` source
func accounts(query: AccountQuery) async throws -> [Account]
```

## Parameters 

`query`  

An AccountQuery that describes the kinds of accounts to look for.

## Return Value

An array of Account structures.

## See Also

### Accounts

func accountHistory(since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Account>

Returns a list of accounts a person added since a time specified by the provided financial history token.

struct AssetAccount

A structure that describes the characteristics of an asset account.

struct LiabilityAccount

A structure that describes the characteristics of a liability account.

enum Account

A structure that describes a financial account.

