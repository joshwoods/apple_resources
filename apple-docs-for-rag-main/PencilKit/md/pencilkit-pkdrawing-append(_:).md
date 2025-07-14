

- PencilKit
- PKDrawing
-  append(\_:) 

Instance Method

# append(\_:)

Appends the contents of the specified drawing object to an existing drawing object that you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
mutating func append(_ toAppend: PKDrawing)
```

## Parameters 

`toAppend`  

A drawing object that contains additional content.

## See Also

### Modifying the drawing

func transform(using: CGAffineTransform)

Applies the specified transform to the contents of this drawing.

func transformed(using: CGAffineTransform) -> PKDrawing

Applies the specified transform and returns a new drawing.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

