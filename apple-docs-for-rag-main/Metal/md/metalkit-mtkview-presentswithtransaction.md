

- MetalKit
- MTKView
-  presentsWithTransaction 

Instance Property

# presentsWithTransaction

A Boolean value that determines whether the view presents its content using a Core Animation transaction.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var presentsWithTransaction: Bool { get set }
```

## Discussion

This property mirrors the value on the underlying CAMetalLayer object, and determines whether the view synchronizes updates to its own contents with other content changes in Core Animation. For more information about how this property affects your rendering code, see presentsWithTransaction.

## See Also

### Configuring Drawing Behavior

var preferredFramesPerSecond: Int

The rate at which the view redraws its contents.

var isPaused: Bool

A Boolean value that indicates whether the draw loop is paused.

var enableSetNeedsDisplay: Bool

A Boolean value that indicates whether the view responds to setNeedsDisplay().

func draw()

Redraws the view’s contents immediately.

