

- SwiftUI
- FocusedValue
-  wrappedValue 

Instance Property

# wrappedValue

The value for the focus key given the current scope and state of the focused view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var wrappedValue: Value? { get }
```

## Discussion

Returns `nil` when nothing in the focused view hierarchy exports a value.

