

- SwiftUI
- FocusState
-  wrappedValue 

Instance Property

# wrappedValue

The current state value, taking into account whatever bindings might be in effect due to the current location of focus.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var wrappedValue: Value { get nonmutating set }
```

## Discussion

When focus is not in any view that is bound to this state, the wrapped value will be `nil` (for optional-typed state) or `false` (for `Bool`- typed state).

## See Also

### Inspecting the focus state

var projectedValue: FocusState&lt;Value>.Binding

A projection of the focus state value that returns a binding.

struct Binding

A property wrapper type that can read and write a value that indicates the current focus location.

