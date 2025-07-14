

- SwiftUI
- HorizontalAlignment
-  listRowSeparatorLeading 

Type Property

# listRowSeparatorLeading

A guide marking the leading edge of a `List` row separator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static let listRowSeparatorLeading: HorizontalAlignment
```

## Discussion

Use this guide to align the leading end of the bottom `List` row separator with any other horizontal guide of a view that is part of the cell content.

The following example shows the row separator aligned with the leading edge of the `Text` containing the name of food:

```
List {
    ForEach(favoriteFoods) { food in
        HStack {
            Text(food.emoji)
                .font(.system(size: 40))
            Text(food.name)
                .alignmentGuide(.listRowSeparatorLeading) {
                    $0[.leading]
                }
        }
    }
}
```

To change the visibility or tint of the row separator use respectively listRowSeparator(_:edges:) and listRowSeparatorTint(_:edges:).

## See Also

### Getting guides

static let leading: HorizontalAlignment

A guide that marks the leading edge of the view.

static let center: HorizontalAlignment

A guide that marks the horizontal center of the view.

static let trailing: HorizontalAlignment

A guide that marks the trailing edge of the view.

static let listRowSeparatorTrailing: HorizontalAlignment

A guide marking the trailing edge of a `List` row separator.

