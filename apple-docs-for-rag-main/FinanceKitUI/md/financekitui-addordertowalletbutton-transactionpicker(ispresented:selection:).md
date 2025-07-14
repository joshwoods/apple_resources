

- FinanceKitUI
- AddOrderToWalletButton
-  transactionPicker(isPresented:selection:) 

Instance Method

# transactionPicker(isPresented:selection:)

Presents a picker that selects a collection of transactions.

FinanceKitUISwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func transactionPicker(
    isPresented: Binding,
    selection: Binding
) -> some View
```

## Parameters 

`isPresented`  

The binding to whether the transaction picker should be shown.

`selection`  

The selection of transactions from the transaction picker.

