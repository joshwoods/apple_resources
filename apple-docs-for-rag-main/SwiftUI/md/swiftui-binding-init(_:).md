

- SwiftUI
- Binding
-  init(\_:) 

Initializer

# init(\_:)

Creates a binding by projecting the base value to a hashable value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ base: Binding) where Value == AnyHashable, V : Hashable
```

Show all declarations

## Parameters 

`base`  

A `Hashable` value to project to an `AnyHashable` value.

## See Also

### Creating a binding

init(projectedValue: Binding&lt;Value>)

Creates a binding from the value of another binding.

init(get:set:)

Creates a binding with closures that read and write the binding value.

static func constant(Value) -> Binding&lt;Value>

Creates a binding with an immutable value.

