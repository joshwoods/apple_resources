

- AppKit
- NSImage
-  hitTest(\_:withDestinationRect:context:hints:flipped:) 

Instance Method

# hitTest(\_:withDestinationRect:context:hints:flipped:)

Returns whether the destination rectangle would intersect a non-transparent portion of the image.

macOS 10.6+

``` source
func hitTest(
    _ testRectDestSpace: NSRect,
    withDestinationRect imageRectDestSpace: NSRect,
    context: NSGraphicsContext?,
    hints: [NSImageRep.HintKey : Any]?,
    flipped: Bool
) -> Bool
```

## Parameters 

`testRectDestSpace`  

The rectangle to hit test.

`imageRectDestSpace`  

A rectangle representing the drawn size of the image.

`context`  

A graphics context. This value can be `nil`.

`hints`  

An optional dictionary of hints that provide more context for selecting or generating a `CGImage`, and may override properties of the `referenceContext`. See `Image Hint Dictionary Keys` for a summary of the possible key-value pairs.

`flipped`  

true if the image is flipped, otherwise false.

## Return Value

YES if the `testRectDestSpace` intersects with non-transparent content within the `imageRectDestSpace`, otherwise NO.

## Discussion

This method simulates the results of hit-testing the test rectangle as if the image was drawn in the graphics context using the provided hints and respecting the specified flippedness.

