

- SwiftUI
- LayoutSubview
-  priority 

Instance Property

# priority

The layout priority of the subview.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var priority: Double { get }
```

## Discussion

If you define a custom layout type using the Layout protocol, you can read this value from subviews and use the value when deciding how to assign space to subviews. For example, you can read all of the subview priorities into an array before placing the subviews in a custom layout type called `BasicVStack`:

```
extension BasicVStack {
    func placeSubviews(
        in bounds: CGRect,
        proposal: ProposedViewSize,
        subviews: Subviews,
        cache: inout ()
    ) {
        let priorities = subviews.map { subview in
            subview.priority
        }

        // Place views, based on priorities.
    }
}
```

Set the layout priority for a view that appears in your layout by applying the layoutPriority(_:) view modifier. For example, you can assign two different priorities to views that you arrange with `BasicVStack`:

```
BasicVStack {
    Text("High priority")
        .layoutPriority(10)
    Text("Low priority")
        .layoutPriority(1)
}
```

## See Also

### Getting subview characteristics

func dimensions(in: ProposedViewSize) -> ViewDimensions

Asks the subview for its dimensions and alignment guides.

func sizeThatFits(ProposedViewSize) -> CGSize

Asks the subview for its size.

var spacing: ViewSpacing

The subviews’s preferred spacing values.

