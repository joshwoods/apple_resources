

- SwiftUI
-  Canvas 

Structure

# Canvas

A view type that supports immediate mode drawing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Canvas where Symbols : View
```

## Overview

Use a canvas to draw rich and dynamic 2D graphics inside a SwiftUI view. The canvas passes a GraphicsContext to the closure that you use to perform immediate mode drawing operations. The canvas also passes a CGSize value that you can use to customize what you draw. For example, you can use the context’s stroke(_:with:lineWidth:) command to draw a Path instance:

```
Canvas { context, size in
    context.stroke(
        Path(ellipseIn: CGRect(origin: .zero, size: size)),
        with: .color(.green),
        lineWidth: 4)
}
.frame(width: 300, height: 200)
.border(Color.blue)
```

The example above draws the outline of an ellipse that exactly inscribes a canvas with a blue border:

In addition to outlined and filled paths, you can draw images, text, and complete SwiftUI views. To draw views, use the init(opaque:colorMode:rendersAsynchronously:renderer:symbols:) method to supply views that you can reference from inside the renderer. You can also add masks, apply filters, perform transforms, control blending, and more. For information about how to draw, see GraphicsContext.

A canvas doesn’t offer interactivity or accessibility for individual elements, including for views that you pass in as symbols. However, it might provide better performance for a complex drawing that involves dynamic data. Use a canvas to improve performance for a drawing that doesn’t primarily involve text or require interactive elements.

## Topics

### Creating a canvas

init(opaque: Bool, colorMode: ColorRenderingMode, rendersAsynchronously: Bool, renderer: (inout GraphicsContext, CGSize) -> Void)

Creates and configures a canvas.

init(opaque: Bool, colorMode: ColorRenderingMode, rendersAsynchronously: Bool, renderer: (inout GraphicsContext, CGSize) -> Void, symbols: () -> Symbols)

Creates and configures a canvas that you supply with renderable child views.

### Managing opacity and color

var isOpaque: Bool

A Boolean that indicates whether the canvas is fully opaque.

var colorMode: ColorRenderingMode

The working color space and storage format of the canvas.

### Referencing symbols

var symbols: Symbols

A view that provides child views that you can use in the drawing callback.

### Rendering

var rendersAsynchronously: Bool

A Boolean that indicates whether the canvas can present its contents to its parent view asynchronously.

var renderer: (inout GraphicsContext, CGSize) -> Void

The drawing callback that you use to draw into the canvas.

## Relationships

### Conforms To

- Copyable
- View

  Conforms when `Symbols` conforms to `View`.

## See Also

### Immediate mode drawing

Add Rich Graphics to Your SwiftUI App

Make your apps stand out by adding background materials, vibrancy, custom graphics, and animations.

struct GraphicsContext

An immediate mode drawing destination, and its current state.

