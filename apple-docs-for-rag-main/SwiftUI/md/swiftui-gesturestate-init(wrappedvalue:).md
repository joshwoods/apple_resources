

- SwiftUI
- GestureState
-  init(wrappedValue:) 

Initializer

# init(wrappedValue:)

Creates a view state that’s derived from a gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(wrappedValue: Value)
```

## Parameters 

`wrappedValue`  

A wrapped value for the gesture state property.

## See Also

### Creating a gesture state

init(initialValue: Value)

Creates a view state that’s derived from a gesture with an initial value.

init(initialValue: Value, reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with an initial state value and a closure that provides a transaction to reset it.

init(initialValue: Value, resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with an initial state value and a transaction to reset it.

init(reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with a closure that provides a transaction to reset it.

init(resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with a transaction to reset it.

init(wrappedValue: Value, reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with a wrapped state value and a closure that provides a transaction to reset it.

init(wrappedValue: Value, resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with a wrapped state value and a transaction to reset it.

