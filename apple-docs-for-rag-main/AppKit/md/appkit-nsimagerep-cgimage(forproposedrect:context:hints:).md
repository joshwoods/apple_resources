

- AppKit
- NSImageRep
-  cgImage(forProposedRect:context:hints:) 

Instance Method

# cgImage(forProposedRect:context:hints:)

Returns a Core Graphics image object that captures the drawing of the image.

macOS 10.6+

``` source
func cgImage(
    forProposedRect proposedDestRect: UnsafeMutablePointer?,
    context: NSGraphicsContext?,
    hints: [NSImageRep.HintKey : Any]?
) -> CGImage?
```

## Parameters 

`proposedDestRect`  

On input, the proposed destination rectangle for drawing the image. If `nil`, it defaults to the smallest pixel-integral rectangle containing `{{0,0}, self.size}`. The `proposedDestRect` is in user space in the reference context.

On output, the `proposedDestRect` may have been altered. This is because a CGImage is necessarily pixel-integral, while an NSImage is not. In order to produce a CGImage for rect `(0.5, 0.5, 4.0, 4.0)` without distortion or double-antialiasing, we may have to produce a 5x5 `CGImage`, and also inflate the `proposedDestRect`. Drawing the `CGImage` in the out-value `proposedDestRect` is the same as drawing the NSImage in the in-value of proposed rect.

`context`  

A graphics context. Can be `nil`.

`hints`  

An optional dictionary of hints that provide more context for selecting or generating the image. See NSImageRep.HintKey for a summary of the possible key-value pairs.

## Return Value

A CGImage. This may be an existing CGImage if one is available. If not, a new CGImage is created.

## Discussion

An NSImage is potentially resolution independent, and may have representations that allow it to draw well in many contexts. A CGImage is more like a single pixel-based representation. This method produces a snapshot of how the NSImage would draw if it was asked to draw in the proposed rectangle in the graphics context.

All input parameters are optional. They provide hints for how to choose among existing CGImage objects, or how to create one if there isn’t already a CGImage available. The parameters are only hints.

This method is intended as an override point for image representation subclasses that naturally have a CGImage available. For example, NSBitmapImageRep overrides it to return the CGImage that naturally backs the representation. You don’t need to override the method except possibly for performance, though. The NSImageRep-level implementation will produce a CGImage by making a buffer and calling draw(). That’s likely to be the best possible implementation for reps that aren’t naturally CGImage-backed. The draw() method remains the only method of NSImageRep that a subclasser really needs to override.

