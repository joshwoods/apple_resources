

- SwiftUI
- Transaction
-  scrollTargetAnchor 

Instance Property

# scrollTargetAnchor

The preferred alignment of the view within a scroll view’s visible region when scrolling to a view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var scrollTargetAnchor: UnitPoint? { get set }
```

## Discussion

Use this API in conjunction with a `ScrollViewProxy/scrollTo(_:anchor)` or when updating the binding provided to a scrollPosition(id:anchor:).

```
@Binding var position: Item.ID?

var body: some View {
    ScrollView {
        LazyVStack {
            ForEach(items) { item in
                ItemView(item)
            }
        }
        .scrollTargetLayout()
    }
    .scrollPosition(id: $position)
    .safeAreaInset(edge: .bottom) {
        Button("Scroll To Bottom") {
            withAnimation {
                withTransaction(\.scrollTargetAnchor, .bottom) {
                    position = items.last?.id
                }
            }
        }
    }
}
```

When used with the scrollPosition(id:anchor:) modifier, this value will be preferred over the anchor specified in the modifier for the current transaction.

## See Also

### Getting information about a transaction

var isContinuous: Bool

A Boolean value that indicates whether the transaction originated from an action that produces a sequence of values.

var tracksVelocity: Bool

Whether this transaction will track the velocity of any animatable properties that change.

subscript&lt;K>(K.Type) -> K.Value

Accesses the transaction value associated with a custom key.

