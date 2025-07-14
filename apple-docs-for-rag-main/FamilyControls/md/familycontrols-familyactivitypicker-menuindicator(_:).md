

- FamilyControls
- FamilyActivityPicker
-  menuIndicator(\_:) 

Instance Method

# menuIndicator(\_:)

Sets the menu indicator visibility for controls within this view.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
nonisolated
func menuIndicator(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

The menu indicator visibility to apply.

## Discussion

Use this modifier to override the default menu indicator visibility for controls in this view. For example, the code below creates a menu without an indicator:

```
Menu {
    ForEach(history , id: \.self) { historyItem in
        Button(historyItem.title) {
            self.openURL(historyItem.url)
        }
    }
} label: {
    Label("Back", systemImage: "chevron.backward")
        .labelStyle(.iconOnly)
} primaryAction: {
    if let last = history.last {
        self.openURL(last.url)
    }
}
.menuIndicator(.hidden)
```

Note

On tvOS, the standard button styles do not include a menu indicator, so this modifier will have no effect when using a built-in button style. You can implement an indicator in your own `ButtonStyle` implementation by checking the value of the `menuIndicatorVisibility` environment value.

## See Also

### Visibility

func hidden() -> some View

Hides this view unconditionally.

func labelsHidden() -> some View

Hides the labels of any controls contained within this view.

func listRowSeparator(Visibility, edges: VerticalEdge.Set) -> some View

Sets the display mode for the separator associated with this specific row.

func listSectionSeparator(Visibility, edges: VerticalEdge.Set) -> some View

Sets whether to hide the separator associated with a list section.

