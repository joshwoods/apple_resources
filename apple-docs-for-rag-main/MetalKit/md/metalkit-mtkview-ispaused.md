

- MetalKit
- MTKView
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates whether the draw loop is paused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isPaused: Bool { get set }
```

## Discussion

If the value is false, the view periodically redraws the contents, at a frame rate set by the value of preferredFramesPerSecond.

The default value is false.

## See Also

### Configuring Drawing Behavior

var preferredFramesPerSecond: Int

The rate at which the view redraws its contents.

var enableSetNeedsDisplay: Bool

A Boolean value that indicates whether the view responds to setNeedsDisplay().

func draw()

Redraws the view’s contents immediately.

var presentsWithTransaction: Bool

A Boolean value that determines whether the view presents its content using a Core Animation transaction.

