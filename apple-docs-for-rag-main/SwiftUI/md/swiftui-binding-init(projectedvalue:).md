

- SwiftUI
- Binding
-  init(projectedValue:) 

Initializer

# init(projectedValue:)

Creates a binding from the value of another binding.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(projectedValue: Binding)
```

## See Also

### Creating a binding

init(_:)

Creates a binding by projecting the base value to a hashable value.

init(get:set:)

Creates a binding with closures that read and write the binding value.

static func constant(Value) -> Binding&lt;Value>

Creates a binding with an immutable value.

