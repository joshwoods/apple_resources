

- ManagedAppDistribution
- ManagedAppView
-  listRowSeparatorTint(\_:edges:) 

Instance Method

# listRowSeparatorTint(\_:edges:)

Sets the tint color associated with a row.

ManagedAppDistributionSwiftUIiOS 15.0+iPadOS 15.0+macOS 13.0+

``` source
nonisolated
func listRowSeparatorTint(
    _ color: Color?,
    edges: VerticalEdge.Set = .all
) -> some View
```

## Parameters 

`color`  

The color to use to tint the row separators, or `nil` to use the default color for the current list style.

`edges`  

The set of row edges for which the tint applies. The list style might decide to not display certain separators, typically the top edge. The default is `VerticalEdge/Set/all`.

## Discussion

Separators can be presented above and below a row. You can specify to which edge this preference should apply.

This modifier expresses a preference to the containing `List`. The list style is the final arbiter for the separator tint.

The following example shows a simple grouped list whose row separators are tinted based on row-specific data:

```
List {
    ForEach(garage.cars) { car in
        Text(car.model)
            .listRowSeparatorTint(car.brandColor)
    }
}
.listStyle(.grouped)
```

To hide a row separators, use `View/listRowSeparator(_:edges:)`. To hide or change the tint color for a section separator, use `View/listSectionSeparator(_:edges:)` and `View/listSectionSeparatorTint(_:edges:)`.

