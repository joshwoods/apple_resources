

- SwiftUI
- Binding
-  init(get:set:) 

Initializer

# init(get:set:)

Creates a binding with closures that read and write the binding value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
init(
    get: @escaping @isolated(any) () -> Value,
    set: @escaping @isolated(any) (Value) -> Void
)
```

Show all declarations

## Parameters 

`get`  

A closure that retrieves the binding value. The closure has no parameters, and returns a value.

`set`  

A closure that sets the binding value. The closure has the following parameter:

- newValue: The new value of the binding value.

## Discussion

A binding conforms to Sendable only if its wrapped value type also conforms to Sendable. It is always safe to pass a sendable binding between different concurrency domains. However, reading from or writing to a binding’s wrapped value from a different concurrency domain may or may not be safe, depending on how the binding was created. SwiftUI will issue a warning at runtime if it detects a binding being used in a way that may compromise data safety.

For a “computed” binding created using get and set closure parameters, the safety of accessing its wrapped value from a different concurrency domain depends on whether those closure arguments are isolated to a specific actor. For example, a computed binding with closure arguments that are known (or inferred) to be isolated to the main actor must only ever access its wrapped value on the main actor as well, even if the binding is also sendable.

## See Also

### Creating a binding

init(_:)

Creates a binding by projecting the base value to a hashable value.

init(projectedValue: Binding&lt;Value>)

Creates a binding from the value of another binding.

static func constant(Value) -> Binding&lt;Value>

Creates a binding with an immutable value.

