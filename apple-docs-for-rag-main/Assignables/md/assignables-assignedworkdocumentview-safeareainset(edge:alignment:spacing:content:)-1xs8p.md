

- Assignables
- AssignedWorkDocumentView
-  safeAreaInset(edge:alignment:spacing:content:) 

Instance Method

# safeAreaInset(edge:alignment:spacing:content:)

Shows the specified content beside the modified view.

AssignablesSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func safeAreaInset(
    edge: HorizontalEdge,
    alignment: VerticalAlignment = .center,
    spacing: CGFloat? = nil,
    @ViewBuilder content: () -> V
) -> some View where V : View
```

## Parameters 

`edge`  

The horizontal edge of the view to inset by the width of `content`, to make space for `content`.

`spacing`  

Extra distance placed between the two views, or nil to use the default amount of spacing.

`alignment`  

The alignment guide used to position `content` vertically.

`content`  

A view builder function providing the view to display in the inset space of the modified view.

## Return Value

A new view that displays `content` beside the modified view, making space for the `content` view by horizontally insetting the modified view.

## Discussion

The `content` view is anchored to the specified horizontal edge in the parent view, aligning its vertical axis to the specified alignment guide. The modified view is inset by the width of `content`, from `edge`, with its safe area increased by the same amount.

```
struct ScrollableViewWithSideBar: View {
    var body: some View {
        ScrollView {
            ScrolledContent()
        }
        .safeAreaInset(edge: .leading, spacing: 0) {
            SideBarContent()
        }
    }
}
```

