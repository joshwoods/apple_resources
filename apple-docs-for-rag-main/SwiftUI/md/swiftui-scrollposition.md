

- SwiftUI
-  ScrollPosition 

Structure

# ScrollPosition

A type that defines the semantic position of where a scroll view is scrolled within its content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ScrollPosition
```

## Overview

Use this type along with the `View/scrollPosition(_:)` modifier to control where a scroll view is positioned. You can use this type to scroll in a variety of ways:

- scroll to a view with a provided identity

- scroll to a concrete offset

- scroll to an edge

You can create a scroll position with a specified view identity type

```
@State private var position = ScrollPosition(idType: MyItem.ID.self)
```

SwiftUI will use that along with the views in the scroll view’s scroll target layout to programmatically scroll to those views and to update the viewID property as the user scrolls. Use the `View/scrollTargetLayout()` modifier to configure which layout contains your scroll targets.

When scrolling to a view with an identifier, SwiftUI will update the position with the value of the top-most view scrolled within the visible region of the scroll view.

In the following example, the position binding will update to reflect the top-most ItemView as the scroll view scrolls.

```
@Binding var items: [MyItem]
@State private var position: ScrollPosition
    = .init(idType: MyItem.ID.self)

ScrollView {
    LazyVStack {
        ForEach(items) { item in
            ItemView(item)
        }
    }
    .scrollTargetLayout()
}
.scrollPosition($scrolledID)
```

You can then query the currently scrolled id by using the viewID(type:).

```
let viewID: MyItem.ID = position.viewID(type: MyItem.ID.self)
```

While most use cases will use view identity based scrolling, you can also use the scroll position type to scroll to offsets or edges. For example, you can create a button that scrolls to the bottom of the scroll view by specifying an edge.

```
Button("Scroll to bottom") {
    position.scrollTo(edge: .bottom)
}
```

When configuring a scroll position, SwiftUI will attempt to keep that position stable. For an edge, that means keeping a top aligned scroll view scrolled to the top if the content size changes. For a point, SwiftUI won’t attempt to keep that exact offset scrolled when the content size changes nor will it update to a new offset when that changes.

For view identity positions, SwiftUI will attempt to keep the view with the identity specified in the provided binding visible when events occur that might cause it to be scrolled out of view by the system. Some examples of these include:

- The data backing the content of a scroll view is re-ordered.

- The size of the scroll view changes, like when a window is resized on macOS or during a rotation on iOS.

- The scroll view initially lays out it content defaulting to the top most view, but the binding has a different view’s identity.

You can provide an anchor to a view identity based position to:

- Influence which view the system chooses as the view whose identity value will update the providing binding as the scroll view scrolls.

- Control the alignment of the view when scrolling to a view when writing a new binding value.

In the example below, the bottom most view will be chosen to update the position binding with.

```
ScrollView {
    LazyVStack {
        ForEach(items) { item in
            ItemView(item)
        }
    }
    .scrollTargetLayout()
}
.scrollPosition($scrolledID, anchor: .bottom)
```

For example, providing a value of bottom will prefer to have the bottom-most view chosen and prefer to scroll to views aligned to the bottom.

If no anchor has been provided, SwiftUI will scroll the minimal amount when using the scroll position to programmatically scroll to a view.

## Topics

### Initializers

init(id: some Hashable &amp; Sendable, anchor: UnitPoint?)

Creates a new scroll position to a view with a provided identity value.

init(idType: (some Hashable &amp; Sendable).Type)

Creates a new automatic scroll position.

init(idType: (some Hashable &amp; Sendable).Type, edge: Edge)

Creates a new scroll position to be scrolled to the provided edge.

init(idType: (some Hashable &amp; Sendable).Type, point: CGPoint)

Creates a new scroll position to be scrolled to the provided point.

init(idType: (some Hashable &amp; Sendable).Type, x: CGFloat)

Creates a new scroll position to be scrolled to the provided y value.

init(idType: (some Hashable &amp; Sendable).Type, x: CGFloat, y: CGFloat)

Creates a new scroll position to be scrolled to the provided x value.

init(idType: (some Hashable &amp; Sendable).Type, y: CGFloat)

Creates a new scroll position to be scrolled to the provided y value.

### Instance Properties

var edge: Edge?

The positioned edge of the scroll view if configured to be in that position.

var isPositionedByUser: Bool

Whether the scroll view has been positioned by the user.

var point: CGPoint?

The positioned point of the scroll view if configured to be in that position.

var viewID: (any Hashable &amp; Sendable)?

The type-erased id of the view positioned in the scroll view if configured to be in that position or the user has scrolled past a view with an id of matching type.

### Instance Methods

func scrollTo(edge: Edge)

Scrolls the position of the scroll view to the edge you provide.

func scrollTo(id: some Hashable &amp; Sendable, anchor: UnitPoint?)

Scrolls the position of the scroll view to a view with a identity value and anchor you provide.

func scrollTo(point: CGPoint)

Scrolls the position of the scroll view to the point you provide.

func scrollTo(x: CGFloat)

Scrolls the position of the scroll view to the x value you provide.

func scrollTo(x: CGFloat, y: CGFloat)

Scrolls the position of the scroll view to the x and y value you provide.

func scrollTo(y: CGFloat)

Scrolls the position of the scroll view to the y value you provide.

func viewID&lt;T>(type: T.Type) -> T?

The id of the view positioned in the scroll view if configured to be in that position or the user has scrolled past a view with an id of matching type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Managing scroll position

func scrollPosition(Binding&lt;ScrollPosition>, anchor: UnitPoint?) -> some View

Associates a binding to a scroll position with a scroll view within this view.

func scrollPosition(id: Binding&lt;(some Hashable)?>, anchor: UnitPoint?) -> some View

Associates a binding to be updated when a scroll view within this view scrolls.

func defaultScrollAnchor(UnitPoint?) -> some View

Associates an anchor to control which part of the scroll view’s content should be rendered by default.

func defaultScrollAnchor(UnitPoint?, for: ScrollAnchorRole) -> some View

Associates an anchor to control the position of a scroll view in a particular circumstance.

struct ScrollAnchorRole

A type defining the role of a scroll anchor.

