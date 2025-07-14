

- AppKit
- NSCustomImageRep
-  init(size:flipped:drawingHandler:) 

Initializer

# init(size:flipped:drawingHandler:)

Initializes a representation of an image of the specified size and flipped status, using a block to draw its content.

macOS 10.8+

``` source
init(
    size: NSSize,
    flipped drawingHandlerShouldBeCalledWithFlippedContext: Bool,
    drawingHandler: @escaping (NSRect) -> Bool
)
```

## Parameters 

`size`  

The size of the image.

`drawingHandlerShouldBeCalledWithFlippedContext`  

true if the drawing handler should be called with a flipped graphics context; otherwise false.

`drawingHandler`  

A block that draws the image representation content in the provided graphics context.

The block may be invoked whenever and on whatever thread the image itself is drawn on. Care should be taken to ensure that all state accessed within the drawingHandler block is done so in a thread safe manner.

This Block replaces the lockFocus() and unlockFocus() technique of creating drawing content. The block is invoked at draw time, the drawing can be adjusted to suit the destination’s pixel density, color space, and other properties.

## Return Value

An initialized NSCustomImageRep object, or `nil` if the object could not be initialized.

## Discussion

Using the this method ensures you’ll get correct results under standard and high resolution.

Like other non-bitmap image rep types, drawing is cached as appropriate for the destination context. Practically speaking, the `drawingHandler` block will be invoked the first time the image is drawn to a particular type of destination (1x or 2x screen, for example). Subsequent drawing operations to the same type of destination will reuse the previously generated bitmap.

## See Also

### Related Documentation

var drawingHandler: ((NSRect) -> Bool)?

The destination rectangle of the drawing handler block.

### Creating Representations of Images in Custom Formats

init(draw: Selector, delegate: Any)

Returns a representation of an image initialized with the specified delegate information.

