

- FamilyControls
- FamilyActivityPicker
-  listSectionSeparatorTint(\_:edges:) 

Instance Method

# listSectionSeparatorTint(\_:edges:)

Sets the tint color associated with a section.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+

``` source
nonisolated
func listSectionSeparatorTint(
    _ color: Color?,
    edges: VerticalEdge.Set = .all
) -> some View
```

## Parameters 

`color`  

The color to use to tint the section separators, or `nil` to use the default color for the current list style.

`edges`  

The set of row edges for which the tint applies. The list style might decide to not display certain separators, typically the top edge. The default is `VerticalEdge/Set/all`.

## Discussion

Separators can be presented above and below a section. You can specify to which edge this preference should apply.

This modifier expresses a preference to the containing `List`. The list style is the final arbiter for the separator tint.

The following example shows a simple grouped list whose section separators are tinted based on section-specific data:

```
List {
    ForEach(garage) { garage in
        Section(header: Text(garage.location)) {
            ForEach(garage.cars) { car in
                Text(car.model)
                    .listRowSeparatorTint(car.brandColor)
            }
        }
        .listSectionSeparatorTint(
            garage.cars.last?.brandColor, edges: .bottom)
    }
}
.listStyle(.grouped)
```

To change the visibility and tint color for a row separator, use `View/listRowSeparator(_:edges:)` and `View/listRowSeparatorTint(_:edges:)`. To hide a section separator, use `View/listSectionSeparator(_:edges:)`.

## See Also

### Tint Color

func tint(Color?) -> some View

Sets the tint color within this view.

func listRowSeparatorTint(Color?, edges: VerticalEdge.Set) -> some View

Sets the tint color associated with a row.

func listItemTint(ListItemTint?) -> some View

Sets the tint effect for content in a list.

func listItemTint(Color?) -> some View

Sets a fixed tint color for content in a list.

