

- FinanceKit
- FinanceStore
-  saveOrder(signedArchive:) 

Instance Method

# saveOrder(signedArchive:)

Adds an order to the store or updates an existing order.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func saveOrder(signedArchive: Data) async throws -> FinanceStore.SaveOrderResult
```

## Discussion

`Data` must be the archive data of a valid, signed order.

## See Also

### Orders

struct FullyQualifiedOrderIdentifier

A structure that specifies the characteristics of an order.

struct HistoryToken

A structure that describes the starting point to use for financial data queries.

