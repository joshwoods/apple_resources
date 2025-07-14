

- SwiftUI
- AccessibilityFocusState
-  projectedValue 

Instance Property

# projectedValue

A projection of the state value that can be used to establish bindings between view content and accessibility focus placement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var projectedValue: AccessibilityFocusState.Binding { get }
```

## Discussion

Use `projectedValue` in conjunction with accessibilityFocused(_:equals:) to establish bindings between view content and accessibility focus placement.

## See Also

### Getting the state

var wrappedValue: Value

The current state value, taking into account whatever bindings might be in effect due to the current location of focus.

struct Binding

