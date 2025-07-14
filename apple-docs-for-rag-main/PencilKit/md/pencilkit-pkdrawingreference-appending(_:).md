

- PencilKit
- PKDrawingReference
-  appending(\_:) 

Instance Method

# appending(\_:)

Returns a new drawing created by appending the current drawing with another drawing you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func appending(_ drawing: PKDrawing) -> PKDrawing
```

## Parameters 

`drawing`  

A drawing object that contains additional content.

## Return Value

A new drawing created by merging the content from the current object with the content in the `drawing` parameter.

## See Also

### Modifying the drawing

func applying(CGAffineTransform) -> PKDrawing

Returns a new drawing object by applying the specified transform to a copy of the current object’s contents.

func appendingStrokes([PKStroke]) -> PKDrawing

Returns a copy of the current drawing with the strokes you provide appended.

