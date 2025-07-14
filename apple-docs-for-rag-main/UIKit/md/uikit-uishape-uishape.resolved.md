

- UIKit
- UIShape
-  UIShape.Resolved 

Structure

# UIShape.Resolved

A shape that has completely resolved based on a context.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
struct Resolved
```

## Topics

### Creating a resolved shape by applying insets

func inset(by: UIEdgeInsets) -> UIShape.Resolved

Creates a new modified shape by applying the provided insets to this shape.

func inset(by: CGFloat) -> UIShape.Resolved

Creates a new modified shape by applying the provided inset to this shape.

### Accessing the resolved shape’s attributes

let shape: UIShape

The abstract shape that produces this resolved shape.

var boundingRect: CGRect

The bounding rectangle that frames the shape.

var path: UIBezierPath

The Bézier path representing this shape.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable

## See Also

### Creating a dynamic hover shape

init(some UIShapeProvider)

Creates a dynamic shape that resolves using the provided resolver closure and resolution context.

protocol UIShapeProvider

An interface for a type that provides a custom shape by resolving it dynamically based on a context.

struct ResolutionContext

The context for resolving a dynamic shape.

