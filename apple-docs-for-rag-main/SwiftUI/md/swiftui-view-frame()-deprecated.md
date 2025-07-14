

- SwiftUI
- View
-  frame() Deprecated

Instance Method

# frame()

Positions this view within an invisible frame.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+Mac Catalyst 13.0+

``` source
nonisolated
func frame() -> some View
```

Deprecated

Use frame(width:height:alignment:) or frame(minWidth:idealWidth:maxWidth:minHeight:idealHeight:maxHeight:alignment:) instead.

## See Also

### Layout modifiers

func edgesIgnoringSafeArea(Edge.Set) -> some View

Changes the view’s proposed area to extend outside the screen’s safe areas.

Deprecated

func coordinateSpace&lt;T>(name: T) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

Deprecated

