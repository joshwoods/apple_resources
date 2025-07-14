

- PencilKit
- PKDrawingReference
-  applying(\_:) 

Instance Method

# applying(\_:)

Returns a new drawing object by applying the specified transform to a copy of the current object’s contents.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func applying(_ transform: CGAffineTransform) -> PKDrawing
```

## Parameters 

`transform`  

The transform to apply to the drawing.

## Return Value

A new drawing created by applying the specified `transform` to the current object.

## See Also

### Modifying the drawing

func appendingStrokes([PKStroke]) -> PKDrawing

Returns a copy of the current drawing with the strokes you provide appended.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

