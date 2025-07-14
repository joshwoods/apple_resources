

- SwiftUI
- FocusedBinding
-  projectedValue 

Instance Property

# projectedValue

A binding to the optional value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var projectedValue: Binding { get }
```

## Discussion

The unwrapped value is `nil` when no focused view hierarchy has published a corresponding binding.

## See Also

### Getting the value

var wrappedValue: Value?

The unwrapped value for the focus key given the current scope and state of the focused view hierarchy.

