

- FinanceKitUI
- AddOrderToWalletButton
-  lineLimit(\_:) 

Instance Method

# lineLimit(\_:)

Sets to a partial range the number of lines that text can occupy in this view.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func lineLimit(_ limit: PartialRangeThrough) -> some View
```

## Parameters 

`limit`  

The line limit.

## Discussion

Use this modifier to specify a partial range of lines that a `Text` view or a vertical `TextField` can occupy. When the text of such views occupies more space than the provided limit, a `Text` view truncates its content while a `TextField` becomes scrollable.

```
Form {
    TextField("Title", text: $model.title)
    TextField("Notes", text: $model.notes, axis: .vertical)
        .lineLimit(...3)
}
```

