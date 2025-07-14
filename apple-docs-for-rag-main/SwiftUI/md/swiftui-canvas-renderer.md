

- SwiftUI
- Canvas
-  renderer 

Instance Property

# renderer

The drawing callback that you use to draw into the canvas.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var renderer: (inout GraphicsContext, CGSize) -> Void
```

## Parameters 

`context`  

The graphics context to draw into.

`size`  

The current size of the view.

## See Also

### Rendering

var rendersAsynchronously: Bool

A Boolean that indicates whether the canvas can present its contents to its parent view asynchronously.

