

- SwiftUI
- View
-  contentShape(\_:eoFill:) 

Instance Method

# contentShape(\_:eoFill:)

Defines the content shape for hit testing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func contentShape(
    _ shape: S,
    eoFill: Bool = false
) -> some View where S : Shape
```

## Parameters 

`shape`  

The hit testing shape for the view.

`eoFill`  

A Boolean that indicates whether the shape is interpreted with the even-odd winding number rule.

## Return Value

A view that uses the given shape for hit testing.

## See Also

### Controlling hit testing

func allowsTightening(Bool) -> some View

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

func contentShape&lt;S>(ContentShapeKinds, S, eoFill: Bool) -> some View

Sets the content shape for this view.

struct ContentShapeKinds

A kind for the content shape of a view.

