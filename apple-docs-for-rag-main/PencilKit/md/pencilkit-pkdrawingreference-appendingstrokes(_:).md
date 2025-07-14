

- PencilKit
- PKDrawingReference
-  appendingStrokes(\_:) 

Instance Method

# appendingStrokes(\_:)

Returns a copy of the current drawing with the strokes you provide appended.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func appendingStrokes(_ strokes: [PKStroke]) -> PKDrawing
```

## Parameters 

`strokes`  

An array of strokes to append to this drawing.

## Return Value

A new drawing created by appending the provided strokes to the current drawing.

## See Also

### Modifying the drawing

func applying(CGAffineTransform) -> PKDrawing

Returns a new drawing object by applying the specified transform to a copy of the current object’s contents.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

