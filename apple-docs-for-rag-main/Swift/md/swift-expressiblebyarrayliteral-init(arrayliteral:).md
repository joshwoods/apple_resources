

- Swift
- ExpressibleByArrayLiteral
-  init(arrayLiteral:) 

Initializer

# init(arrayLiteral:)

Creates an instance initialized with the given elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(arrayLiteral elements: Self.ArrayLiteralElement...)
```

**Required** Default implementations provided.

## Default Implementations

### ExpressibleByArrayLiteral Implementations

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init(arrayLiteral: Self.Scalar...)

Creates a vector from the specified elements.

