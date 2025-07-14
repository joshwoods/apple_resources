

- PencilKit
- PKDrawing
-  transform(using:) 

Instance Method

# transform(using:)

Applies the specified transform to the contents of this drawing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
mutating func transform(using transform: CGAffineTransform)
```

## Parameters 

`transform`  

The CGAffineTransform to apply when transforming the contents of this drawing.

## See Also

### Modifying the drawing

func transformed(using: CGAffineTransform) -> PKDrawing

Applies the specified transform and returns a new drawing.

func append(PKDrawing)

Appends the contents of the specified drawing object to an existing drawing object that you provide.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

