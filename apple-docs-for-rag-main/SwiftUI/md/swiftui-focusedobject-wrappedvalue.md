

- SwiftUI
- FocusedObject
-  wrappedValue 

Instance Property

# wrappedValue

The underlying value referenced by the focused object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
var wrappedValue: ObjectType? { get }
```

## Discussion

This property provides primary access to the value’s data. However, you don’t access `wrappedValue` directly. Instead, you use the property variable created with the FocusedObject attribute.

When a mutable value changes, the new value is immediately available. However, a view displaying the value is updated asynchronously and may not show the new value immediately.

## See Also

### Getting the value

var projectedValue: FocusedObject&lt;ObjectType>.Wrapper?

A projection of the focused object that creates bindings to its properties using dynamic member lookup.

struct Wrapper

A wrapper around the underlying focused object that can create bindings to its properties using dynamic member lookup.

