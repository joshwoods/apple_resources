

- SwiftUI
- EnvironmentValues
-  layoutDirection 

Instance Property

# layoutDirection

The layout direction associated with the current environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var layoutDirection: LayoutDirection { get set }
```

## Discussion

Use this value to determine or set whether the environment uses a left-to-right or right-to-left direction.

## See Also

### Setting a layout direction

func layoutDirectionBehavior(LayoutDirectionBehavior) -> some View

Sets the behavior of this view for different layout directions.

enum LayoutDirectionBehavior

A description of what should happen when the layout direction changes.

enum LayoutDirection

A direction in which SwiftUI can lay out content.

