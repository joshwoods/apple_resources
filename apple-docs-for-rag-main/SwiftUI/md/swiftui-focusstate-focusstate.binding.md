

- SwiftUI
- FocusState
-  FocusState.Binding 

Structure

# FocusState.Binding

A property wrapper type that can read and write a value that indicates the current focus location.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen @propertyWrapper
struct Binding
```

## Topics

### Inspecting the binding

var projectedValue: FocusState&lt;Value>.Binding

A projection of the binding value that returns a binding.

var wrappedValue: Value

The underlying value referenced by the bound property.

## See Also

### Inspecting the focus state

var projectedValue: FocusState&lt;Value>.Binding

A projection of the focus state value that returns a binding.

var wrappedValue: Value

The current state value, taking into account whatever bindings might be in effect due to the current location of focus.

