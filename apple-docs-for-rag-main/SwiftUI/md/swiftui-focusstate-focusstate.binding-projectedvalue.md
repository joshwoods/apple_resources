

- SwiftUI
- FocusState
- FocusState.Binding
-  projectedValue 

Instance Property

# projectedValue

A projection of the binding value that returns a binding.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var projectedValue: FocusState.Binding { get }
```

## Discussion

Use the projected value to pass a binding value down a view hierarchy.

## See Also

### Inspecting the binding

var wrappedValue: Value

The underlying value referenced by the bound property.

