

- SwiftUI
- ObservedObject
-  ObservedObject.Wrapper 

Structure

# ObservedObject.Wrapper

A wrapper of the underlying observable object that can create bindings to its properties.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @dynamicMemberLookup @preconcurrency @frozen
struct Wrapper
```

## Topics

### Subscripts

subscript&lt;Subject>(dynamicMember _: ReferenceWritableKeyPath&lt;ObjectType, Subject>) -> Binding&lt;Subject>

Gets a binding to the value of a specified key path.

## Relationships

### Conforms To

- Sendable

## See Also

### Getting the value

var wrappedValue: ObjectType

The underlying value that the observed object references.

var projectedValue: ObservedObject&lt;ObjectType>.Wrapper

A projection of the observed object that creates bindings to its properties.

