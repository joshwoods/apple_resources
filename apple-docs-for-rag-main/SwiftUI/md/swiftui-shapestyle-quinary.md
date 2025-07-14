

- SwiftUI
- ShapeStyle
-  quinary 

Type Property

# quinary

A shape style that maps to the fifth level of the current content style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var quinary: HierarchicalShapeStyle { get }
```

Available when `Self` is `HierarchicalShapeStyle`.

## Discussion

This hierarchical style maps to the fifth level of the current foreground style, or to the fifth level of the default foreground style if you haven’t set a foreground style in the view’s environment. You typically set a foreground style by supplying a non-hierarchical style to the foregroundStyle(_:) modifier.

For information about how to use shape styles, see ShapeStyle.

## See Also

### Hierarchical styles

var secondary: some ShapeStyle

Returns the second level of this shape style.

var tertiary: some ShapeStyle

Returns the third level of this shape style.

var quaternary: some ShapeStyle

Returns the fourth level of this shape style.

var quinary: some ShapeStyle

Returns the fifth level of this shape style.

static var primary: HierarchicalShapeStyle

A shape style that maps to the first level of the current content style.

static var secondary: HierarchicalShapeStyle

A shape style that maps to the second level of the current content style.

static var tertiary: HierarchicalShapeStyle

A shape style that maps to the third level of the current content style.

static var quaternary: HierarchicalShapeStyle

A shape style that maps to the fourth level of the current content style.

