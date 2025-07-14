

- SwiftUI
- Binding
-  constant(\_:) 

Type Method

# constant(\_:)

Creates a binding with an immutable value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func constant(_ value: Value) -> Binding
```

## Parameters 

`value`  

An immutable value.

## Discussion

Use this method to create a binding to a value that cannot change. This can be useful when using a PreviewProvider to see how a view represents different values.

```
// Example of binding to an immutable value.
PlayButton(isPlaying: Binding.constant(true))
```

## See Also

### Creating a binding

init(_:)

Creates a binding by projecting the base value to a hashable value.

init(projectedValue: Binding&lt;Value>)

Creates a binding from the value of another binding.

init(get:set:)

Creates a binding with closures that read and write the binding value.

