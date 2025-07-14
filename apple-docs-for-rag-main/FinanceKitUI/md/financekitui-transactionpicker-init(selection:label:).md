

- FinanceKitUI
- TransactionPicker
-  init(selection:label:) 

Initializer

# init(selection:label:)

Creates a picker that selects a collection of transactions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    selection: Binding,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`selection`  

The selection of transactions from the transaction picker.

`label`  

The view that describes the action of choosing transactions.

