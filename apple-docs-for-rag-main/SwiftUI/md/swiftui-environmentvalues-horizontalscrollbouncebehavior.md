

- SwiftUI
- EnvironmentValues
-  horizontalScrollBounceBehavior 

Instance Property

# horizontalScrollBounceBehavior

The scroll bounce mode for the horizontal axis of scrollable views.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
var horizontalScrollBounceBehavior: ScrollBounceBehavior { get set }
```

## Discussion

Use the scrollBounceBehavior(_:axes:) view modifier to set this value in the Environment.

## See Also

### Configuring scroll bounce behavior

func scrollBounceBehavior(ScrollBounceBehavior, axes: Axis.Set) -> some View

Configures the bounce behavior of scrollable views along the specified axis.

var verticalScrollBounceBehavior: ScrollBounceBehavior

The scroll bounce mode for the vertical axis of scrollable views.

struct ScrollBounceBehavior

The ways that a scrollable view can bounce when it reaches the end of its content.

