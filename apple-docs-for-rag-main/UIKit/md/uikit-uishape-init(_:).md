

- UIKit
- UIShape
-  init(\_:) 

Initializer

# init(\_:)

Creates a dynamic shape that resolves using the provided resolver closure and resolution context.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
init(_ provider: some UIShapeProvider)
```

## See Also

### Creating a dynamic hover shape

protocol UIShapeProvider

An interface for a type that provides a custom shape by resolving it dynamically based on a context.

struct ResolutionContext

The context for resolving a dynamic shape.

struct Resolved

A shape that has completely resolved based on a context.

