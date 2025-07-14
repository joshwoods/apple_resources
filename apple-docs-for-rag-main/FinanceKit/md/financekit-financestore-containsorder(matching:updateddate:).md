

- FinanceKit
- FinanceStore
-  containsOrder(matching:updatedDate:) 

Instance Method

# containsOrder(matching:updatedDate:)

Checks whether the finance store contains an order.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func containsOrder(
    matching fqoid: FullyQualifiedOrderIdentifier,
    updatedDate: Date? = nil
) async throws -> FinanceStore.ContainsOrderResult
```

## Discussion

This returns `.notFound` for any orders that the process isn’t entitled to access.

