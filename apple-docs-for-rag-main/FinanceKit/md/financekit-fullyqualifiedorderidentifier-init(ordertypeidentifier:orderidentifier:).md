

- FinanceKit
- FullyQualifiedOrderIdentifier
-  init(orderTypeIdentifier:orderIdentifier:) 

Initializer

# init(orderTypeIdentifier:orderIdentifier:)

Initializes the object with values that uniquely identify an order within an order type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
init(
    orderTypeIdentifier: String,
    orderIdentifier: String
)
```

## Discussion

In combination with the order type identifier, these two properties uniquely identify an order in FinanceStore.

