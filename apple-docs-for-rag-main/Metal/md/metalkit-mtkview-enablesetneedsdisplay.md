

- MetalKit
- MTKView
-  enableSetNeedsDisplay 

Instance Property

# enableSetNeedsDisplay

A Boolean value that indicates whether the view responds to setNeedsDisplay().

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var enableSetNeedsDisplay: Bool { get set }
```

## Discussion

If this value and the value of isPaused are true, the view behaves similarly to a UIView object, responding to calls to setNeedsDisplay(). In this case, the view’s internal draw loop is paused and updates are event-driven instead.

The default value is false.

## See Also

### Configuring Drawing Behavior

var preferredFramesPerSecond: Int

The rate at which the view redraws its contents.

var isPaused: Bool

A Boolean value that indicates whether the draw loop is paused.

func draw()

Redraws the view’s contents immediately.

var presentsWithTransaction: Bool

A Boolean value that determines whether the view presents its content using a Core Animation transaction.

