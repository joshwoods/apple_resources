

- SwiftUI
- GestureState
-  init(initialValue:) 

Initializer

# init(initialValue:)

Creates a view state that’s derived from a gesture with an initial value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(initialValue: Value)
```

## Parameters 

`initialValue`  

An initial value for the gesture state property.

## See Also

### Creating a gesture state

init(initialValue: Value, reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with an initial state value and a closure that provides a transaction to reset it.

init(initialValue: Value, resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with an initial state value and a transaction to reset it.

init(reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with a closure that provides a transaction to reset it.

init(resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with a transaction to reset it.

init(wrappedValue: Value)

Creates a view state that’s derived from a gesture.

init(wrappedValue: Value, reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with a wrapped state value and a closure that provides a transaction to reset it.

init(wrappedValue: Value, resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with a wrapped state value and a transaction to reset it.

