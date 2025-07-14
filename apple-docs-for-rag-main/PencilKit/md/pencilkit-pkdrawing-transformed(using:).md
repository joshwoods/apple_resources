

- PencilKit
- PKDrawing
-  transformed(using:) 

Instance Method

# transformed(using:)

Applies the specified transform and returns a new drawing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
func transformed(using transform: CGAffineTransform) -> PKDrawing
```

## Parameters 

`transform`  

The CGAffineTransform to apply to the contents of this drawing.

## Return Value

A new drawing with the provided `transform` applied.

## See Also

### Modifying the drawing

func transform(using: CGAffineTransform)

Applies the specified transform to the contents of this drawing.

func append(PKDrawing)

Appends the contents of the specified drawing object to an existing drawing object that you provide.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

