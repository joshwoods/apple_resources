

- SwiftUI
- Transaction
-  isContinuous 

Instance Property

# isContinuous

A Boolean value that indicates whether the transaction originated from an action that produces a sequence of values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isContinuous: Bool { get set }
```

## Discussion

This value is `true` if a continuous action created the transaction, and is `false` otherwise. Continuous actions include things like dragging a slider or pressing and holding a stepper, as opposed to tapping a button.

## See Also

### Getting information about a transaction

var scrollTargetAnchor: UnitPoint?

The preferred alignment of the view within a scroll view’s visible region when scrolling to a view.

var tracksVelocity: Bool

Whether this transaction will track the velocity of any animatable properties that change.

subscript&lt;K>(K.Type) -> K.Value

Accesses the transaction value associated with a custom key.

