

- UIKit
- UIShape
-  UIShape.ResolutionContext 

Structure

# UIShape.ResolutionContext

The context for resolving a dynamic shape.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
struct ResolutionContext
```

## Topics

### Determining the content shape

var contentShape: UIShape.Resolved

The resolved shape of the content to which this shape can apply.

## See Also

### Creating a dynamic hover shape

init(some UIShapeProvider)

Creates a dynamic shape that resolves using the provided resolver closure and resolution context.

protocol UIShapeProvider

An interface for a type that provides a custom shape by resolving it dynamically based on a context.

struct Resolved

A shape that has completely resolved based on a context.

