

- SwiftUI
- EnvironmentObject
-  EnvironmentObject.Wrapper 

Structure

# EnvironmentObject.Wrapper

A wrapper of the underlying environment object that can create bindings to its properties using dynamic member lookup.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @dynamicMemberLookup @frozen @preconcurrency
struct Wrapper
```

## Topics

### Getting a binding value

subscript&lt;Subject>(dynamicMember _: ReferenceWritableKeyPath&lt;ObjectType, Subject>) -> Binding&lt;Subject>

Returns a binding to the resulting value of a given key path.

## Relationships

### Conforms To

- Sendable

## See Also

### Getting the value

var wrappedValue: ObjectType

The underlying value referenced by the environment object.

var projectedValue: EnvironmentObject&lt;ObjectType>.Wrapper

A projection of the environment object that creates bindings to its properties using dynamic member lookup.

