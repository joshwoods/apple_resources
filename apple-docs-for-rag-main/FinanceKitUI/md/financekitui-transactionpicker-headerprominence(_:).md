

- FinanceKitUI
- TransactionPicker
-  headerProminence(\_:) 

Instance Method

# headerProminence(\_:)

Sets the header prominence for this view.

FinanceKitUISwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func headerProminence(_ prominence: Prominence) -> some View
```

## Parameters 

`prominence`  

The prominence to apply.

## Discussion

In the following example, the section header appears with increased prominence:

```
List {
    Section(header: Text("Header")) {
        Text("Row")
    }
    .headerProminence(.increased)
}
.listStyle(.insetGrouped)
```

