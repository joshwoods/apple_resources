

- UIKit
-  UIShape 

Structure

# UIShape

An abstract representation of a shape.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
struct UIShape
```

## Overview

A UIShape can represent different types of shapes, including:

- A simple shape like a rectangle or circle that resolves into a concrete shape according to context (like size and position)

- A Bézier path

- A dynamic shape that resolves using a custom closure

You typically use a UIShape with APIs like UIHoverStyle to represent the shape of an effect.

## Topics

### Creating a hover shape

static var rect: UIShape

Creates a rectangular shape.

static var capsule: UIShape

Creates a capsule shape, a rounded rectangle with a corner radius equal to half the length of the rectangle’s smallest edge.

static var circle: UIShape

Creates a circular shape, with a radius equal to half the length of the frame rectangle’s smallest edge.

static func rect(cornerRadius: CGFloat, cornerCurve: UICornerCurve, maskedCorners: UIRectCorner) -> UIShape

Creates a rectangular shape with rounded corners, using the provided corner radius, corner curve, and rectangle corners.

static func fixedRect(CGRect, cornerRadius: CGFloat, cornerCurve: UICornerCurve, maskedCorners: UIRectCorner) -> UIShape

Creates a fixed rectangular shape that uses the provided rectangle as its shape, regardless of the frame that contains it.

enum UICornerCurve

The corner curve to apply to a view.

### Creating a hover shape from a custom path

static func path(UIBezierPath) -> UIShape

Creates a shape with a custom Bézier path.

### Creating a dynamic hover shape

init(some UIShapeProvider)

Creates a dynamic shape that resolves using the provided resolver closure and resolution context.

protocol UIShapeProvider

An interface for a type that provides a custom shape by resolving it dynamically based on a context.

struct ResolutionContext

The context for resolving a dynamic shape.

struct Resolved

A shape that has completely resolved based on a context.

### Creating a shape by applying insets

func inset(by: UIEdgeInsets) -> UIShape

Creates a new modified shape by applying the provided insets to this shape.

func inset(by: CGFloat) -> UIShape

Creates a new modified shape by applying the provided inset to this shape.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- UIShapeProvider

## See Also

### Specifying a hover shape

var shape: UIShape?

The shape to use for the hover effect.

