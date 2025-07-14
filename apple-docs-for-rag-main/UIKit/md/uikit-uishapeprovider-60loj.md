

- UIKit
-  UIShapeProvider 

Protocol

# UIShapeProvider

An interface for a type that provides a custom shape by resolving it dynamically based on a context.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
protocol UIShapeProvider : Equatable
```

## Topics

### Resolving a custom shape

func resolve(in: Self.Context) -> Self.Resolved

Resolves the shape in the provided context.

**Required**

### Supporting types

typealias Context

The context for resolving a dynamic shape.

typealias Resolved

A shape that has completely resolved based on a context.

## Relationships

### Inherits From

- Equatable

### Conforming Types

- UIShape

## See Also

### Creating a dynamic hover shape

init(some UIShapeProvider)

Creates a dynamic shape that resolves using the provided resolver closure and resolution context.

struct ResolutionContext

The context for resolving a dynamic shape.

struct Resolved

A shape that has completely resolved based on a context.

