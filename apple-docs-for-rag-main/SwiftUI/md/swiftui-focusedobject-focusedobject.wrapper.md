

- SwiftUI
- FocusedObject
-  FocusedObject.Wrapper 

Structure

# FocusedObject.Wrapper

A wrapper around the underlying focused object that can create bindings to its properties using dynamic member lookup.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency @dynamicMemberLookup @frozen
struct Wrapper
```

## Topics

### Accessing members

subscript&lt;T>(dynamicMember _: ReferenceWritableKeyPath&lt;ObjectType, T>) -> Binding&lt;T>

Returns a binding to the value of a given key path.

## See Also

### Getting the value

var projectedValue: FocusedObject&lt;ObjectType>.Wrapper?

A projection of the focused object that creates bindings to its properties using dynamic member lookup.

var wrappedValue: ObjectType?

The underlying value referenced by the focused object.

