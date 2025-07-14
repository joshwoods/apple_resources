

- RealityKit
- RealityViewDefaultPlaceholder
-  defaultScrollAnchor(\_:for:) 

Instance Method

# defaultScrollAnchor(\_:for:)

Associates an anchor to control the position of a scroll view in a particular circumstance.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func defaultScrollAnchor(
    _ anchor: UnitPoint?,
    for role: ScrollAnchorRole
) -> some View
```

## Discussion

You can associate a `UnitPoint` to a `ScrollView` using the `View/defaultScrollAnchor(_:)` modifier. By default, the system uses this point for different kinds of behaviors including:

- Where the scroll view should initially be scrolled

- How the scroll view should handle content size or container size changes

- How the scroll view should align content smaller than its container size

You can further customize this behavior by assigning different unit points for these different cases.

For example, you can use the `View/defaultScrollAnchor(_:)` modifier to provide a value of `UnitPoint/bottom` as the anchor for all cases and then opt out of certain cases by providing a different value for them.

```
@Binding var items: [Item]
@Binding var scrolledID: Item.ID?

ScrollView {
    LazyVStack {
        ForEach(items) { item in
            ItemView(item)
        }
    }
}
.defaultScrollAnchor(.bottom)
.defaultScrollAnchor(.topLeading, for: .alignment)
```

