

- SwiftUI
- Shape
-  layoutDirectionBehavior 

Instance Property

# layoutDirectionBehavior

Returns the behavior this shape should use for different layout directions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
var layoutDirectionBehavior: LayoutDirectionBehavior { get }
```

**Required** Default implementation provided.

## Discussion

If the layoutDirectionBehavior for a Shape is one that mirrors, the shape’s path will be mirrored horizontally when in the specified layout direction. When mirrored, the individual points of the path will be transformed.

Defaults to `.mirrors` when deploying on iOS 17.0, macOS 14.0, tvOS 17.0, watchOS 10.0 and later, and to `.fixed` if not. To mirror a path when deploying to earlier releases, either use `View.flipsForRightToLeftLayoutDirection` for a filled or stroked shape or conditionally mirror the points in the path of the shape.

## Default Implementations

### Shape Implementations

var layoutDirectionBehavior: LayoutDirectionBehavior

Returns the behavior this shape should use for different layout directions.

