

- MetalKit
- MTKView
-  draw() 

Instance Method

# draw()

Redraws the view’s contents immediately.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func draw()
```

## Discussion

This method manually tells the view to redraw its contents. Calling this method causes the view to call either the draw(in:) method of the view’s delegate, or the draw(_:) method of the MTKView subclass. Never call this method inside either drawing function.

## See Also

### Configuring Drawing Behavior

var preferredFramesPerSecond: Int

The rate at which the view redraws its contents.

var isPaused: Bool

A Boolean value that indicates whether the draw loop is paused.

var enableSetNeedsDisplay: Bool

A Boolean value that indicates whether the view responds to setNeedsDisplay().

var presentsWithTransaction: Bool

A Boolean value that determines whether the view presents its content using a Core Animation transaction.

